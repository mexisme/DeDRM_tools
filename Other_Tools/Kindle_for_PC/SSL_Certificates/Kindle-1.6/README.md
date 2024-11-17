Older versions of Kindle for PC (e.g. 1.6) rely on an SSL CRT cert that was marked as unsafe and removed from the Global Roots.
Unfortunately, without it, the Kindle App won't connect to Amazon.

To connect, you need to either add the CRT in this directory to your /etc/ssl/certs/ dir, or set the env-var SSL_CERT_FILE to the path of the file before starting Wine / Kindle.

https://askubuntu.com/questions/1323817/kindle-app-unable-to-connect

