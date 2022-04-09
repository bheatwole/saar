# SAAR System Authorization Access Request

! Until there is a way to get the client smartcard to sign some bytes inside a browser, this project is on hold

Web Cryptography API allows for signing, but does not have any certificate discovery calls yet.

## Initial Requirements
- client in Rust+WASM, server in golang: reason, to demonstrate my skills with these techs
- app knows who user is via smartcard
- app allows user to pick a system and request access

## Less Dumb Initial Requirements
- Simple HTML form that asks the exact same fields that are in the PDF
- 'Sign' button downloads a PDF that will show as signed in Adobe Acrobat

## Initial Tasks
- golang server with client cert acceptance
- server rest endpoint accepting post data and returning signed PDF
- server static index.html with post form
