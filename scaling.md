# Scaling

## Definition

**Scaling**  means when we add extra capacity or functionality into an existing product or software it should remain stable while adapting the upgrade and changes with base functionality.

## Need of Scaling

In today’s fast-paced and rapidly evolving technology period User's expectations and Preferences are changing very quickly. When we design any product or Software we must keep the **growth** factor in mind.
Scaling is not a feature or extra functionality of a product it just keeps the product stable and productive in the volatile nature of the industry. from the beginning, it’s easier to design a scalable product. It also saves time and money in the long run. Because we can continue using the same product by just upgrading it. Every time we don’t have to think about effective performance because we design the scalable product.

## Benefit of Scaling

- If the product is scalable we can easily add extra functionality to the product. Without ``redesign`` the entire product with ``effective performance`` and ``base functionality``.

- We can release the different ``Editions`` of our product with different functionality and Sell the different editions to different users according to their usage.

## Principles of Scalability

## FUNCTIONALITY

Fulfiling the demand of the user is a very challenging process. Before adding the extra functionality in the product we must plan out. Is there any need for this functionality or not ?. Do we have the resources to manage this functionality ?.  Can be able to keep the original features ?. If you can manage all this then try to add the extra functionality.

## DATABASE

Manging the user data is the most important part of a product. We must choose the database which is best suitable for our product. Which let the system grow smoothly. There is a trade-off between different databases. We use DB which can manage both scalability and performance of product even with a large dataset.

## CODE

It is an important point which most people neglect while writing the code. You must write the ``clean and readable code`` so that in the future while scaling we  have to work with that code again so we can easily understand what is the functionality of this code. You are not just writing for urself maybe another team member has to work and understand the code. We must write different code for different functionality try not to mix the different code in one place.

> We should not write spaghetti code.
> Use comment for describing the functionality of code.

## MAINTENANCE

Maintenance increase the life-time and smooth running of the product. It improves the user experience.

## Types of scaling

Mainly there are two types of scaling one is ``horizontal scaling``(also known as ``Scaling out``) and another is ``vertical scaling``(also known as ``scaling up``). There is not much difference between the two both done by adding resources. They differ by their implementation and performance.

In horizontal scaling, we add ``extra resources`` in a pool of resources or you can say adding resource parallelly. In vertical scaling adding more ``power(CPU, RAM)`` to an existing system.

![Horizontal Scaling](https://www.section.io/assets/images/blog/featured-images/horizontal-vs-vertical-scaling-diagram.png )
![vertical Scaling](https://www.section.io/assets/images/blog/featured-images/horizontal-vs-vertical-scaling-diagram.png)

## Vertical Scaling

### Pros

- It consumes less power as compared to running multiple servers.
- Managing resources is easy as you need to handle and manage just one system.
- Inter-process communication, therefore, is faster.
- Load balancing is not required like in horizontal scaling.
- Vertical scaling is easier because we don't have to change the logic.

#### Cons

- Single point of hardware failure which can cause full system down.
- Limited scope of upgradeability in the future.
- The cost of implementing vertical scaling  is really expensive

## Horizontal Scaling

### Pros

- Since the load is distributed across multiple systems, horizontal scaling is more resistant to system failure.
- Much cheaper compared to vertical scaling
- Easy to upgrade

### Cons

- Loadbalancer is required to manage the resources.
- More networking equipment such as routers and switches may be needed.

## Decision

If you have a large set of users/data then go for horizontal scaling. If your business manages only limited no. of user/data then go for vertical scaling.

>most of the organization uses the combination of both.

## Loadbalancer

Loadbalancer is an important piece and essential requirement for designing a scalable system. Loadbalancer act as a ``Guard`` which redistribute the requests coming from the user to pool of server and return the correct images, text, and data in a fast and reliable manner.
It also checks the ``health`` of the servers if one server is not accepting the requests or it is faulty then load balancer remove it from the pool of server without the user noticing and without
affecting the actual flow of your application.

> Load balancer generally work on layer 7 and layer 4 o OSI model. Layer 7 load balancing is more CPU‑intensive and Layer 4 load balancer is packet-based.

![Loadbalancer](https://miro.medium.com/max/381/1*2bCPkZZ0o-pcY2uAQbyL4w.png)

## Why load balancing is required?

- To avoid overload of any single resource.
- To increase performance.
- To handle sudden traffic spikes.
- To minimize response time.
- To optimize resource use

## Types of load balancer

Mainly there are two types of loadbalancer hardware-based and software-based. Hardware-based are expensive and suggested for large infrastructure. Software-based is less expensive and flexible and runs on top of available hardware we just have to install into the system.

> Loadbalancer now provides ``security``, ``acceleration``, ``authentication`` in the software load balancer.

## Load Balancing Algorithms

1. **Round Robin Algorithm**
2. **Weighted Round Robin Algorithm**
3. **Least Connections Algorithm**
4. **Random Algorithm**
5. **IP Hash Algorithm**

## References

References | Links
------------ | -------------
Reference 1 | [](https://fullscale.io/blog/what-is-software-scalability/)
reference 2 | [](https://www.conceptatech.com/blog/importance-of-scalability-in-software-design)
Reference 4 | [](http://www.idc-online.com/technical_references/pdfs/information_technology/Basics_of_Scaling_Load_Balancers.pdf)
Reference 5 | [](https://medium.com/@tudip/basic-guide-load-balancing-and-auto-scaling-in-cloud-computing-219a5f0768a)
Reference 6 | [](https://www.nginx.com/resources/glossary/load-balancing/)
Reference 7 | [](https://medium.com/swlh/basics-of-system-design-horizontal-vs-vertical-scaling-7e92fd219909 )
