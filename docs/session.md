elitech-datareader --command set --interval=10 --upper_limit=60.0 --lower_limit=-30.0 \
--station_no=1 --stop_button=y --delay=0.0 --tone_set=y --alarm=x --temp_unit=C \
--temp_calibration=-1.5 --dev_num=1234567890 --encode=utf8 --user_info="UserInfoユーザー情報" /dev/tty.SLAB_USBtoUART

elitech-datareader --command set --stop_button=y


17:24 $ elitech-datareader --command simple-set --interval=10 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:21 $ elitech-datareader --command devinfo --encode=utf8 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
alarm=AlarmSetting.NONE
current=2021-01-07 09:22:03
delay=0.0
dev_num=E20A105655
humi_calibration=0.0
humi_lower_limit=0.0
humi_upper_limit=0.0
last_online=2021-01-07 09:21:50
lower_limit=-30.0
model_no=50
rec_count=21
rec_interval=00:00:10
start_time=2021-01-07 09:18:35
station_no=1
stop_button=StopButton.DISABLE
temp_calibration=0.0
temp_unit=TemperatureUnit.C
tone_set=ToneSet.NONE
upper_limit=60.0
user_info=RC-5 Data Logger
work_sts=WorkStatus.START
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:22 $ elitech-datareader --command latest /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
25	2021-01-07 09:22:35	22.2
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:22 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
1	2021-01-07 09:18:35	19.3
2	2021-01-07 09:18:45	19.4
3	2021-01-07 09:18:55	19.4
4	2021-01-07 09:19:05	19.5
5	2021-01-07 09:19:15	19.5
6	2021-01-07 09:19:25	19.8
7	2021-01-07 09:19:35	19.8
8	2021-01-07 09:19:45	20.1
9	2021-01-07 09:19:55	20.3
10	2021-01-07 09:20:05	20.4
11	2021-01-07 09:20:15	20.5
12	2021-01-07 09:20:25	20.7
13	2021-01-07 09:20:35	20.9
14	2021-01-07 09:20:45	20.9
15	2021-01-07 09:20:55	21.1
16	2021-01-07 09:21:05	21.2
17	2021-01-07 09:21:15	21.4
18	2021-01-07 09:21:25	21.5
19	2021-01-07 09:21:35	21.7
20	2021-01-07 09:21:45	21.8
21	2021-01-07 09:21:55	21.9
22	2021-01-07 09:22:05	22.0
23	2021-01-07 09:22:15	22.1
24	2021-01-07 09:22:25	22.1
25	2021-01-07 09:22:35	22.2
26	2021-01-07 09:22:45	22.2
(bjorn39) ✘-2 ~/Desktop/elitech-datareader [master|✔]
09:28 $ elitech-datareader --command set --stop_button=y /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
target_station_no=1
rec_interval=00:00:10
upper_limit=60.0
lower_limit=-30.0
update_station_no=1
stop_button=StopButton.ENABLE
delay=0.0
tone_set=ToneSet.NONE
alarm=AlarmSetting.NONE
temp_unit=TemperatureUnit.C
temp_calibration=0.0
humi_upper_limit=0.0
humi_lower_limit=0.0
humi_calibration=0.0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]


(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
17:24 $ ls /dev/serial/by-id/
usb-1a86_USB_Serial-if00-port0  usb-Sierra_Wireless_Inc._Sierra_Wireless_EM7345_4G_LTE_013937003638598-if02
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
17:24 $ elitech-datareader --command simple-set --interval=10 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
17:25 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0

(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
08:30 $
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
08:30 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
08:30 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
08:31 $ elitech-datareader --command simple-set --interval=10 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
08:31 $ elitech-datareader --command simple-set --interval=10 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:16 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:16 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:16 $ elitech-datareader --command latest /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:17 $ elitech-datareader --command devinfo --encode=utf8 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
alarm=AlarmSetting.NONE
current=2021-01-07 09:17:48
delay=0.0
dev_num=E20A105655
humi_calibration=0.0
humi_lower_limit=0.0
humi_upper_limit=0.0
last_online=2021-01-07 09:17:20
lower_limit=-30.0
model_no=50
rec_count=0
rec_interval=00:00:10
start_time=2021-01-07 08:31:41
station_no=1
stop_button=StopButton.DISABLE
temp_calibration=0.0
temp_unit=TemperatureUnit.C
tone_set=ToneSet.NONE
upper_limit=60.0
user_info=RC-5 Data Logger
work_sts=WorkStatus.NOT_START
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:17 $ elitech-datareader --command devinfo --encode=utf8 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
alarm=AlarmSetting.NONE
current=2021-01-07 09:21:50
delay=0.0
dev_num=E20A105655
humi_calibration=0.0
humi_lower_limit=0.0
humi_upper_limit=0.0
last_online=2021-01-07 09:17:49
lower_limit=-30.0
model_no=50
rec_count=20
rec_interval=00:00:10
start_time=2021-01-07 09:18:35
station_no=1
stop_button=StopButton.DISABLE
temp_calibration=0.0
temp_unit=TemperatureUnit.C
tone_set=ToneSet.NONE
upper_limit=60.0
user_info=RC-5 Data Logger
work_sts=WorkStatus.START
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:21 $
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:21 $ elitech-datareader --command devinfo --encode=utf8 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
alarm=AlarmSetting.NONE
current=2021-01-07 09:22:03
delay=0.0
dev_num=E20A105655
humi_calibration=0.0
humi_lower_limit=0.0
humi_upper_limit=0.0
last_online=2021-01-07 09:21:50
lower_limit=-30.0
model_no=50
rec_count=21
rec_interval=00:00:10
start_time=2021-01-07 09:18:35
station_no=1
stop_button=StopButton.DISABLE
temp_calibration=0.0
temp_unit=TemperatureUnit.C
tone_set=ToneSet.NONE
upper_limit=60.0
user_info=RC-5 Data Logger
work_sts=WorkStatus.START
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:22 $ elitech-datareader --command latest /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
25	2021-01-07 09:22:35	22.2
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:22 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
1	2021-01-07 09:18:35	19.3
2	2021-01-07 09:18:45	19.4
3	2021-01-07 09:18:55	19.4
4	2021-01-07 09:19:05	19.5
5	2021-01-07 09:19:15	19.5
6	2021-01-07 09:19:25	19.8
7	2021-01-07 09:19:35	19.8
8	2021-01-07 09:19:45	20.1
9	2021-01-07 09:19:55	20.3
10	2021-01-07 09:20:05	20.4
11	2021-01-07 09:20:15	20.5
12	2021-01-07 09:20:25	20.7
13	2021-01-07 09:20:35	20.9
14	2021-01-07 09:20:45	20.9
15	2021-01-07 09:20:55	21.1
16	2021-01-07 09:21:05	21.2
17	2021-01-07 09:21:15	21.4
18	2021-01-07 09:21:25	21.5
19	2021-01-07 09:21:35	21.7
20	2021-01-07 09:21:45	21.8
21	2021-01-07 09:21:55	21.9
22	2021-01-07 09:22:05	22.0
23	2021-01-07 09:22:15	22.1
24	2021-01-07 09:22:25	22.1
25	2021-01-07 09:22:35	22.2
26	2021-01-07 09:22:45	22.2
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:22 $
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:22 $ elitech-datareader --command set --stop_button=y
usage: description Elitech RC-4 / RC-5 data reader [-h] [-c {init,get,latest,simple-set,set,devinfo,clock,raw}] [-i INTERVAL]
                                                   [--upper_limit UPPER_LIMIT] [--lower_limit LOWER_LIMIT]
                                                   [--station_no STATION_NO] [--stop_button {y,n}]
                                                   [--delay {0.0,0.5,1.0,1.5,2.0,2.5,3.0,3.5,4.0,4.5,5.0,5.5,6.0}]
                                                   [--tone_set {y,n}] [--alarm {x,3,10}] [--temp_unit {C,F}]
                                                   [--temp_calibration TEMP_CALIBRATION] [--humi_upper_limit HUMI_UPPER_LIMIT]
                                                   [--humi_lower_limit HUMI_LOWER_LIMIT] [--humi_calibration HUMI_CALIBRATION]
                                                   [--time TIME] [--dev_num DEV_NUM] [--user_info USER_INFO] [--encode ENCODE]
                                                   [--page_size PAGE_SIZE] [--req REQ] [--res_len RES_LEN] [--value_only]
                                                   [--ser_baudrate SER_BAUDRATE] [--ser_timeout SER_TIMEOUT]
                                                   serial_port
description Elitech RC-4 / RC-5 data reader: error: the following arguments are required: serial_port
(bjorn39) ✘-2 ~/Desktop/elitech-datareader [master|✔]
09:28 $ elitech-datareader --command set --stop_button=y /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
target_station_no=1
rec_interval=00:00:10
upper_limit=60.0
lower_limit=-30.0
update_station_no=1
stop_button=StopButton.ENABLE
delay=0.0
tone_set=ToneSet.NONE
alarm=AlarmSetting.NONE
temp_unit=TemperatureUnit.C
temp_calibration=0.0
humi_upper_limit=0.0
humi_lower_limit=0.0
humi_calibration=0.0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:28 $








(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:28 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:29 $ elitech-datareader --command latest /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:29 $ elitech-datareader --command devinfo --encode=utf8 /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
alarm=AlarmSetting.NONE
current=2021-01-07 09:29:47
delay=0.0
dev_num=E20A105655
humi_calibration=0.0
humi_lower_limit=0.0
humi_upper_limit=0.0
last_online=2021-01-07 09:29:39
lower_limit=-30.0
model_no=50
rec_count=0
rec_interval=00:00:10
start_time=2021-01-07 09:18:35
station_no=1
stop_button=StopButton.ENABLE
temp_calibration=0.0
temp_unit=TemperatureUnit.C
tone_set=ToneSet.NONE
upper_limit=60.0
user_info=RC-5 Data Logger
work_sts=WorkStatus.NOT_START
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:29 $ elitech-datareader --command get /dev/serial/by-id/usb-1a86_USB_Serial-if00-port0
1	2021-01-07 09:30:44	22.0
2	2021-01-07 09:30:54	22.2
3	2021-01-07 09:31:04	22.2
4	2021-01-07 09:31:14	22.1
(bjorn39) ✔ ~/Desktop/elitech-datareader [master|✔]
09:31 $
