---
date: 2021-03-19T20:32
title: Feedback in communication
slug: Feedback1
tags:
  - ti
  - assignment
---

# Role of feedback in Communication

## 6 possible role for feedback in communication

- correct receiver misunderstanding ?
- predict and correct the noise ? 
- cooperate with other senders ?
- determine properties of the channel ?
- reduce communication delay ? 
- reduce computational complexity at the transmitter or the receiver and improve communication rate ? 

# Feedback for memmoryless channel

![feedback](static/1617509790.png)

``````
Memoryless channel = the statistical result at current receiver(y) only influenced by current transmitter so there's no memory
``````

let's assume there is a system where there is an transmitter(x) and a receiver(y), and the conditional mass function of the system is p(y|x). if one wish
to use this channel n times, then 

## Kesimpulan

- Feedback reduce code complexity
  - Proof : X => {0,1} , y => {0,1,E}, dimana E menyimbolkan penghapusan kompleksitas
  - anggap y= x; {P = 1-@} dan y = E; {P = @} C = 1-@ susah dicapai sedangkan menggunakan non feedback

# Feedback on gaussian channel

Gaussian channel where channel is time-discrete, and noise were present. the result of receiver(y) is influenced not only by current x but also by W and 
past x. there's also power constraint.

## Kesimpulan

- Feedback at most double the capacity at the gaussian channel ( Cfb <= 2Cfnb )
- Cfb = Cfnb + 1/2 bits/transmission
- Feedback can predict the noise thanks to Y (backward process) so it can determine the Zi = Yi-X, and because the noise not independent so it cn predict the noice location  

# Unknown Channel

Assume Input were X = {1,2,...,m} and Y = {0,1}, so all input except i were crushed into 0, with using feedback the transmitter know where does to put the i into 1, because of the feedback 

# Multiple Access channel

if sender and receiver were not one (x1,x2,...,xn) and one receiver y, so the conditional distribution were p(y|x1,x2,...,xn), so there were also interference between the sender
so the capacity is classified as region as following, 
R1 

# Computational complexity for mutiple access channel

consider the binary erasure multiple access channel in wich X1,X2 => {0,1}; Y => {0,1,2} and X = X1 + X2
![complexity](./static/1617619013.png)

