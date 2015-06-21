OpenVPN for Android
=============

Description
------------
With the new VPNService of Android API level 14+ (Ice Cream Sandwhich) it is possible to create a VPN service that does not root access. This project is a port of OpenVPN.

Read the README
---------------
If you want to develop on ics-openvpn please read the [doc/README.txt](http://code.google.com/p/ics-openvpn/source/browse/doc/README.txt) *before* opening issues or emailing me. 

You can help
------------
Even if you are no programmer you can help by translating the OpenVPN client into your native language. [Crowdin provides a free service for non commercial open source projects](http://crowdin.net/project/ics-openvpn/invite) (Fixing/completing existing translations is very welcome as well)

FAQ
-----
You can find the FAQ here (same as in app): http://code.google.com/p/ics-openvpn/wiki/FAQ

Note to administrators
------------------------

You make your life and that of your users easier if you embed the certificates into the .ovpn file. You or the users can mail the .ovpn as a attachment to the phone and directly import and use it. Also downloading and importing the file works. The MIME Type should be application/x-openvpn-profile. 

Inline files are supported since OpenVPN 2.1rc1 and documented in the  [OpenVPN 2.3 man page](https://community.openvpn.net/openvpn/wiki/Openvpn23ManPage) (under INLINE FILE SUPPORT) 

(Using inline certifaces can also make your life on non Android platforms easier since you have only one file.)

For example `ca mycafile.pem` becomes

  <ca>
  -----BEGIN CERTIFICATE-----
  MIIHPTCCBSWgAwIBAgIBADANBgkqhkiG9w0BAQQFADB5MRAwDgYDVQQKEwdSb290
  [...]
  -----END CERTIFICATE-----
  </ca>

Fotnotes
-----------
Please that OpenVPN used by this project is under GPLv2. 

If you cannot or do not want to use the Play Store you can [download the apk files directly](http://plai.de/android/) . 

If you want to donate you can donate to [arne-paypal@rfc2549.org via paypal](https://www.paypal.com/cgi-bin/webscr?hosted_button_id=R2M6ZP9AF25LS&cmd=_s-xclick).


The old official or main repository was a Mercurial (hg) repository at http://code.google.com/p/ics-openvpn/source/

The new git repository is now at GitHub under https://github.com/schwabe/ics-openvpn

Please read the doc/README before asking question or starting development.