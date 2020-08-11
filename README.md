# Clinic

##Project details:

appointment-service: The server part of the two micro services which takes input of specialization and lists the doctors and their timings

reception: The reception service where you enquire about doctors using specialization(Orthopedics/Gynacologist/General) and timings(AN/FN)

clinic-eureka-zuul-server: Runs on 8765 and registers itself as a eureka client

clinit-eureka-server: Eureka server running on 8761 to which one or more instances of appointment-service and reception service registers.

##How to run:

Run eureka server, then zuul.

Make multiple instances of appointment service and reception using run configuration and start them.

You can use either postman or simple browser to invoke the get requests on reception or appointment-service