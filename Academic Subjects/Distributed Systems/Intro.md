
 A loose definition of **Distributed Systems** according to the text books is:

> A distributed system is a collection of independent computers that appears to its users as a single coherent system.

or

> A set of co-operating computers communicating with each other over a network to get some coherent task done

Examples where Distributed Systems are used:
- Storage for large websites
- Big Data computations over multiple computers
- Peer-to-peer file sharing

A lot of infrastructure is built using distributed systems,
Infrastructure which either NEEDS more than 1 computer to get it's job done, or an infrastructure which inherently is supposed to be spread across multiple physical computers.

> If possible, always try to get things done on a single computer
> Make a distributed system only if necessary.



In order to support heterogeneous computers, i.e different CPU architectures, varying word size, varying Endianness, etc. and networks while offering a single-system view, distributed systems are often organized by means of a layer of software-that is, logically placed between a higher-level layer consisting of users and applications, and a layer underneath consisting of operating systems and basic communication facilities, as shown in the figure



![[Distributed System.png]]





Why do we need Distributed Systems?

1. You need high performance/high parallelism, one single computer has got a great logical CPU, which has multiple cores (sort of physical CPUs), which provide actual parallelism, and now each core has multiple threads for providing much more concurrency on each of these parallelly working cores.

And yet, it's still not enough. Think of big tech companies like Google, Facebook, Discord, etc. They cannot handle all of their millions of users on a single computer system no matter how state of the art the components of the computer system are.

2. To build systems which are fault tolerant

> All computer systems are prone to failure, whether it be software or hardware.

So for example, if entire infrastructure is running on a single computer, if the computer fails, then the entire system fails

In a distributed system, may be a part of the system, i.e, one of many computers might fail, but others will be working, this is called ***Partial Failure*** of the system.

3. Physical reasons?, you don't just communicate within your infrastructe, Eg: multiple banks need to communicate to provide bank tranfers across them, they need to have some way of co-opertaing

4. Security Reasons: there's some code execution I don't trust to be run on my personal computer, maybe it has a bug which might hurt my system during it's execution, but i need the final results of this code.

So let the code be run on some other computer, my computer and this "server" will communicate over a narrowly defined protocol to only send and receive the request for some code execution and get the result response. This is what [RPC]() is essentially.

