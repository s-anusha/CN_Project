# CN_Project

## DCE-06: Validate the ns-3 implementation of TCP Illinois

### Brief:
TCP Illinois uses a mixed signal of packet loss (primary) and queuing delay (secondary) to calculate the appropriate value of congestion window (cwnd). It uses Additive Increase and Multiplicative Decrease (AIMD) like traditional TCP to adjust the value of its cwnd, but the additive and multiplicative factors are not fixed, instead they are a function of average queuing delay. In this project, the aim is to validate ns-3 TCP Illinois implementation by comparing the results obtained from it to those obtained by simulating Linux TCP Illinois.

### Reading:
- [Direct Code Execution] (https://www.nsnam.org/overview/projects/direct-code-execution/ “Direct Code Execution”)
- [Linux kernel code] (https://elixir.bootlin.com/linux/v4.4/source/net/ipv4/tcp_illinois.c “Linux kernel code”)
- [TCP Illinois Paper] (https://www.sciencedirect.com/science/article/pii/S0166531607001307 “TCP Illinois Paper”)
- ns-3 code for TCP Illinois (Path: ns-3.xx/src/internet/model/tcp-illinois.{h, cc})
