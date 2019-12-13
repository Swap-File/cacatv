# cacatv building for Raspbian Buster Lite
```
git clone git://anongit.freedesktop.org/git/gstreamer/gst-plugins-good
cd gst-plugins-good
git checkout d88d1b0
```
Put files in /home/pi/gst-plugins-good/ext/libcaca/
```
./autogen.sh --disable-gtk-doc
make
sudo cp /home/pi/gst-plugins-good/ext/libcaca/.libs/libgstcacasink.so /usr/lib/arm-linux-gnueabihf/gstreamer-1.0/libgstcacasink.so
```
