#!/bin/bash
current_ip=`/usr/bin/dig +short myip.opendns.com @resolver1.opendns.com`
last_ip=`cat current_ip`

#cmp --silent  mynewip || differ=1

if [ "$current_ip" != "$last_ip" ]
then
	/usr/bin/pushbullet push LGE note "Tu nueva IP: $current_ip"
        echo $current_ip > current_ip
fi		

