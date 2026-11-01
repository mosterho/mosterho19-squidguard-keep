##  Use the folowing to create my personalized image
FROM ubuntu/squid:latest

RUN apt update
RUN apt -y full-upgrade
RUN apt -y install nano wget squidguard tzdata

RUN chown -R proxy:proxy /var/lib/squidguard
#COPY update-blacklist.sh /usr/src/
#COPY update-blacklist-part2.sh /usr/src/

#RUN build_cron_job.sh

#ENTRYPOINT ["squid"]
#CMD ["-sNY"]
CMD ["squid", "-sNY"]

