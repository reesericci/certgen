# [certgen](https://github.com/reesericci/certgen)
Bash interactive script for generating SSL certificates with OpenSSL. Designed for use with your own CA.

## How to download
Download the certgen file in the root of the [repository](https://github.com/reesericci/certgen).

Then run `chmod a+x certgen` where you downloaded it.

Then move it into a place that's in your $PATH. `/bin` is a good choice.

## How to use
Create a SAN file for your domain.

Then start the script by running `certgen`.

Certgen will then prompt you for things like where to put all the files for the cert, that SAN file, CSR questions and your CA's Root Certficate and Private key.

Once you're finished, just head into the directory you specified, and the files you need will be there. `crt.crt` is the certificate, and `key.pem` is the private 
key. Both of these files are in PEM format. 
