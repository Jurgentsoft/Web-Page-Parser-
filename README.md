# Web-Page-Parser-
Use BeautifulSoup to parse HTML code from a webpage.
from bs4 import BeautifulSoup
import requests

url = 'https://example.com'
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')
print(soup.prettify())
