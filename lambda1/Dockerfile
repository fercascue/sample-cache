#Stage for maven compile
FROM public.ecr.aws/lambda/java:11

COPY opt/lib /var/task/lib
COPY target/classes /var/task/
COPY target /var/task/lib

RUN ls -la /var/task/lib
RUN ls -la /var/task


# Command to run into the CMD for landa execution.
CMD ["es.totalenergies.customersportal.handler.App::handleRequest"]