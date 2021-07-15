# installing-android-studio-script-linux


```
wget -O - https://developer.android.com/studio |   grep -io '<a href=['"'"'"][^"'"'"']*['"'"'"]' |   sed -e 's/^<a href=["'"'"']//i' -e 's/["'"'"']$//i'|grep linux.tar.gz>lock;
wget -i lock;
rm lock;
tar -xf android-studio-ide-202.7486908-linux.tar.gz -C /opt/;
cd /opt/android-studio/bin/;
./studio.sh
