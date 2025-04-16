<h1 align="center">Ordering Transactions with Bounded Unfairness: Definitions, Complexity and Constructions</h1>

<p align="center">
Aggelos Kiayias<sup>1,2</sup>, Nikos Leonardos <sup>3</sup>, Yu Shen<sup>1</sup>
</p>

<p align="center">
<sup>1</sup>University of Edinburgh
<sup>2</sup>IOG
<sup>3</sup>National and Kapodistrian University of Athens
</p>

<p align="center">EUROCRYPT 2024</p>

<p align="center">
    <a href="http://creativecommons.org/licenses/by/4.0/"><img src="https://img.shields.io/badge/License-CC--BY--4.0-bb6688.svg?style=for-the-badge&labelColor=884499" alt="Personal Website"></a>
    <a href="https://link.springer.com/chapter/10.1007/978-3-031-58734-4_2"><img src="https://img.shields.io/badge/Conference-Proceedings-8888cc.svg?style=for-the-badge&labelColor=884499" alt="Conference Proceedings"></a>
    <a href="https://eprint.iacr.org/2023/1253"><img src="https://img.shields.io/badge/Full-Version-ccaa88.svg?style=for-the-badge&labelColor=884499" alt="Full Version"></a>
</p>

This repository contains the LaTeX source of "Ordering Transactions with Bounded Unfairness: Definitions, Complexity and Constructions" at EUROCRYPT 2024.

## Abstract

An important consideration in the context of distributed ledger protocols is fairness in terms of transaction ordering. Recent work [Crypto 2020] revealed a connection of (receiver) order fairness to social choice theory and related impossibility results arising from the Condorcet paradox. As a result of the impossibility, various relaxations of  order fairness were proposed in prior works. Given that distributed ledger protocols, especially those processing smart contracts, must serialize the input transactions, a natural objective is to  minimize the distance (in terms of  number of transactions) between any pair of  unfairly ordered transactions in the output ledger --- a concept we call *bounded unfairness*. In state machine replication (SMR) parlance this asks for minimizing the number of unfair state updates occurring before the processing of any request. This unfairness minimization objective gives rise to a natural class of parametric
order fairness definitions  that has not been studied before. As we observe, previous realizable relaxations of order fairness do not yield good unfairness bounds.

Achieving optimal order fairness in the sense of bounded unfairness turns out to be connected to the graph theoretic properties of the underlying transaction dependency graph and specifically the *bandwidth* metric of strongly connected components in this graph. This gives rise to a specific instance of the definition that we call ``directed bandwidth order-fairness'' which we show that it captures the best possible that any ledger protocol can achieve in terms of bounding unfairness. We prove ordering transactions in this fashion is NP-hard and non-approximable for any constant ratio. Towards realizing the property, we put forth a new distributed ledger protocol called Taxis that achieves directed bandwidth order-fairness. We present two variations, one that matches the property perfectly but (necessarily) lacks in performance and liveness, and another that achieves  liveness and  better complexity while offering a slightly relaxed version of the  property. Finally, we comment on applications of our work to social choice, a direction which we believe to be of independent interest.
