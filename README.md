# docker-dump1090
Docker for dump1090

Usage
-----
* Pull image
				docker pull philalex/docker-dump1090

* Run image
>	docker run --device=/dev/bus/usb/001/005 -p 8080:8080 -t philalex/docker-dump1090
* or in privileged mode
>	docker run --privileged -p 8080:8080 -t philalex/docker-dump1090

How to find your usb device
---------------------------
Run lsusb and find your USB DVB-T
>`Bus `**`002`**` Device `**`017`**`: ID 0bda:2838 Realtek Semiconductor Corp. RTL2838 `**`DVB-T`**`
=> /dev/bus/usb/002/017