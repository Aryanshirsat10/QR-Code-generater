# QR-Code-generater
!pip install pyqrcode

import pyqrcode 

from pyqrcode import QRCode

#String which represent the QR code

s = input("Enter the link of which QR code is required:-")

#Generate QR code

url = pyqrcode.create(s)

#Create and save the png file naming "myqr.png"

url.svg("myqrcode.svg", scale = 8)

print("The QR Code of link provided by your is saved in an image in the directory you are working, have a good day:))")
