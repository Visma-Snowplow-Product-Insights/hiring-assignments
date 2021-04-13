# Recruitment assignment for Software / Data Engineer
This task is intended for candidates applying for a software / data engineer position in the product insights team at the data science tech hub. This assignment is built around some of the technologies used in our production environment.

We are super happy to have you considering a position in our team. The case below should hopefully give you a little insight into some of the most common challenges we face as a team.

## Introduction
The data science department helps Visma teams with various data science related tasks, where our team focuses on delivering *product insights* at scale. To accomplish this we utilize Snowplow (https://github.com/snowplow), Google Cloud services, and Dataform (https://dataform.co/). A big part to deliver this offering is with a layer of microservices, hosted and orchestrated on Kubernetes. This is built so that you can try out and showcase your skills in some of the technologies we use.

What is Snowplow? All in all, it is a service that tracks, collects and stores behavioral data in a database (read more here: https://snowplowanalytics.com/)

## The Challenge
The challenge will demonstrate your knowledge in deploying and managing microservices. We will be using snowplow micro (https://github.com/snowplow-incubator/snowplow-micro-examples#1-local-setup), a super light-weight demo application of the complete Snowplow platform.

Follow the instructions in the snowplow-micro repository.

### Goal:
- Deploy snowplow-micro on your local machine (follow steps 1.1, 1.2, 1.3 in the guide above)
- To validate the microservice, run following command in local terminal:
```
curl -d "&e=pv&page=curl-test&url=http%3A%2F%2Fjust-testing.com&aid=snowplow-test" -X POST http://localhost:9090/com.snowplowanalytics.iglu/v1
```

## Delivery (examples)
- As a forked repository in your Github profile
- As a demo
- As a flow diagram

### Bonus:
- Instead of docker-decompose, run the service with a Kubernetes manifest instead (will require local Kubernetes setup).

## Questions?
If you have questions about the task or would like us to further specify some of the tings written above, you can contact the person who gave you the assignment.
