FROM sebd/telegraf-rpi:latest

ADD telegraf_arm.conf .

RUN rm -f /etc/telegraf/telegraf.conf
RUN mv telegraf_arm.conf telegraf.conf
RUN cp /telegraf.conf /etc/telegraf/

ENTRYPOINT ["/entrypoint.sh"]
CMD ["telegraf"]
