# Raspberry-Pi-4
硬件连接 购买HDMI线 HDMI转VGA（带源）
烧录2018-06-27-raspbian-stretch.img镜像文件，没有任何输出
重新寻找镜像文件Rasp-OpenCV-19-11-8.img成功开机

上网问题 
最初 输入sudo nano /etc/resolv.conf命令来修改配置文件，
     然后将nameserver后面的一系列数字改成8.8.8.8
     不成功
之后 打开 dhcpcd.conf
      sudo nano /etc/dhcpcd.conf

      # fallback to static profile on eth0
      #interface eth0
      #fallback static_eth0
      将这后面的内容都删了
      成功
      附带链接如下：https://blog.csdn.net/chenchen2360060/article/details/84952081?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-2.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-2.control
