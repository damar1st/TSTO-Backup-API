# TSTO-Backup-API
Request presaved TSTO Tokens, Avatars and Landfiles from TSTOLE.DE - for TSTO-Server Developers ONLY

To request a LandFile, you first need to obtain the original token using the email address:

https://tstole.de/newtool/api.php?gettoken=user@email.com

If the token file is available, you will receive a JSON response like this:

{
  "email": "user@email.com",
  "token": "106362698005010525657223466420999999",
  "Longlifetoken": "QVQxOjIuMDozLjA6NzIwOllOVlViS09MYVVZaGZsdE1CNUIzODYzNGh2aDdkOG9qbGpFOjI3MzQ3OnJpZW50"
}

With the email and token, you can now request the LandFile:

https://tstole.de/newtool/api.php?landfile=user@email.com&token=106362698005010525657223466420999999

If the file exists, you will receive a ZIP file in response, which contains the following files:
The LandFile in various modes, the CurrencyFile, and the FriendListFile.
Sample files can be found in the "Samples" folder.

As a third option, you can also request the avatar:

https://tstole.de/newtool/api.php?getAvatar=user@email.com

The avatar will be returned as a PNG response.

Over 2,000 backups have been created by users. However, due to an initial server issue, it’s possible that not all LandFiles are available on the server.

An upload API for LandFiles is also coming soon...

Happy Tapping!
