# 538project
Latinos Finos Project
%pip install pykrakenapi
%pip install krakenx
%pip install python-binance

import json
from binance.helpers import round_step_size
from datetime import datetime
import pytz
import math
import numpy as np
import krakenex
from pykrakenapi import KrakenAPI
api = krakenex.API()
kraken = KrakenAPI(api)

import urllib.parse
import hashlib
import hmac
import base64

def get_kraken_signature(urlpath, data, secret):

    postdata = urllib.parse.urlencode(data)
    encoded = (str(data['nonce']) + postdata).encode()
    message = urlpath.encode() + hashlib.sha256(encoded).digest()

    mac = hmac.new(base64.b64decode(secret), message, hashlib.sha512)
    sigdigest = base64.b64encode(mac.digest())
    return sigdigest.decode()

#Get account balance

import time
import os
import requests

# Read Kraken API key and secret stored in environment variables
api_url = "https://api.kraken.com"
api_key = 'Tb+yw8lskq4OSljs+juTv6QIZMx+xHK9nyq1me4jOtCGwWPBmQkAaKnS'
api_sec = 'MetILiQE+9uxTGlaP3H932/Sx8agWtroXdythQX/BQMIjJdGV682uC8uQUq3qdJ2nkTq1NdRkNd6dj7i7Fn7jw=='

# Attaches auth headers and returns results of a POST request
def kraken_request(uri_path, data, api_key, api_sec):
    headers = {}
    headers['API-Key'] = api_key
    # get_kraken_signature() as defined in the 'Authentication' section
    headers['API-Sign'] = get_kraken_signature(uri_path, data, api_sec)            
    req = requests.post((api_url + uri_path), headers=headers, data=data)
    return req
