import requests


URL = 'https://kad.arbitr.ru/'
headers = {
    'scheme': 'https',
    'host': 'kad.arbitr.ru',
    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:104.0) Gecko/20100101 Firefox/104.0'
    }
headers_for_list = {
    'scheme': 'https',
    'host': 'kad.arbitr.ru',
    'filename': '/Kad/SearchInstances',
    'Accept': '*/*',
    'Accept-Encoding': 'gzip, deflate, br',
    'Accept-Language': 'ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3',
    'Connection': 'keep-alive',
    'Content-Length': '128',
    'Content-Type': 'application/json',
    'Origin': 'https://kad.arbitr.ru',
    'Referer': 'https://kad.arbitr.ru/',
    'Sec-Fetch-Dest': 'empty',
    'Sec-Fetch-Mode': 'cors',
    'Sec-Fetch-Site': 'same-origin',
    'TE': 'trailers',
    'x-date-format': 'iso',
    'X-Requested-With': 'XMLHttpRequest',
    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:104.0) Gecko/20100101 Firefox/104.0'
    }
payload = {
    'Sides': [{'0':{'Name': '7722467407', 'Type': -1, 'ExactMatch': 'false'}}],
    'Judges': [], "Courts":[], "CaseNumbers":[],
    "Page":1, "Count":25, "DateFrom" :"null", "DateTo": "null"
    }
s = requests.Session()
response1 = s.post(URL, headers=headers)
response2 = s.post(URL, headers=headers_for_list, data=payload)
print(response1.text)
print(response2.text)
