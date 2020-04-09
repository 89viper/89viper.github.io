---
title: Ubuntu18.04.04 login problem
categories: programming
tags: Linux, Ubuntu
---

포맷 직후 우분투 로그인 시, 멈춤 및 꺼짐 현상 해결 방법<br/>(NVIDIA 그래픽 카드 드라이버 문제)

<!-- more -->

# Ubuntu login problem

## 문제

포맷 직후 우분투(Ubuntu-18.04.04-LTS) 로그인 시, 멈춤 및 꺼짐 현상<br/>

## 원인

NIVIDIA 그래픽 카드 드라이버 문제

## 해결 방법

1. 우분투 부팅시 shift, esc를 눌러서 recovery mode로 부팅
2. Grub에서 enter / Network에서 enter / Root에서 enter
3. 추천 드라이버 확인
```
$ ubuntu-drivers devices
```
4. 드라이버 설치 후 리부팅
```
$ sudo add-apt-repository ppa:graphics-drivers/ppa
```
```
$ sudo apt update
```
```
$ sudo apt-get install nvidia-driver-435
```
```
$ sudo reboot
```
