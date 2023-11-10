# QR_code
import qrcode
qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode_constants_ERROR_CORRECT_L,
    box_size=10,
    border=4,
)
qr.add_data("url")
qr.make(fit=True)

img = qr.make_image(fill_color="black", back_color="white")
img.save("qrcode.png")


## install pillow
