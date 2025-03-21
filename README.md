Hey There 

This is a Python project to generate QR code of any link 

In this project I have used Flask framework which is one of the micro web framework written in python.
Apart from Flask I have used python library- QRCODE
This is the customized from of the library:
qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=10,
    border=4,
)
qr.add_data('Some data')
qr.make(fit=True)
img = qr.make_image(fill_color="black", back_color="white")
