#Stage for maven compile
FROM public.ecr.aws/lambda/java:11

RUN ls -la ./opt/lib
COPY ./opt/lib /var/task/lib
RUN ls -la /var/task/lib



# Command to run into the CMD for landa execution.
CMD ["es.totalenergies.customersportal.handler.App::handleRequest"]