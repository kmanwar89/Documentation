http://www.mike-stirling.com/redmine/projects/webradio/wiki/Installation

mkdir ~/SDR
Cd ~/SDR
git clone http://www.mike-stirling.com/git/webradio.git
Sudo apt-get install automake autoconf
Autoreconf --install
./configure
Got error about libmicrohttpd
Sudo apt-get install libmicrohttpd10
Failed on error for libmicrohttpd.  Fuck it.
