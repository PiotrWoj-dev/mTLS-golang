Ressouce used for this project: https://github.com/haoel/mTLS

Then convert and export the certificate to your browser:

cat client.a.crt  client.a.key > client.a.pkcs12.pem

openssl pkcs12 -in client.a.pkcs12.pem -export -out client.a.pkcs12.p12 # convert it into pkcs12 format

Then import the .p12 file in your browser to be able to access the website.