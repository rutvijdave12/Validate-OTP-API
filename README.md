# Validate-OTP-API

API URL and Request/ response is in request.http file

{
    "requestId": "123456543", - random requestId for logging purpose. Needs to be passed by frontend.
    "otpRequestId": "wertyuiyr23", - random otpRequestId needs to be passed during OTP generation and validation.
    "channelId": "LOGIN_MFA", - Pass this channel only.
    "otp": "lsrjXOipsCRBeL8o5JZsLOG4OFcjqWprg4hYzdbKCh4=" - SHA256 hash of the otp string with Base64 encoding should be passed. Use CryptoJS.SHA256(enteredOTP).toString(CryptoJS.enc.Base64) of crypto-js lib in react.
}