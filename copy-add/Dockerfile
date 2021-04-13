FROM centos

RUN yum install httpd -y
ENV contenido prueba;
COPY app /var/www/html
RUN echo "$contenido" > /var/www/html/prueba.html
COPY run.sh  /run.sh
CMD sh /run.sh