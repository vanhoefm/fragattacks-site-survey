---
layout: singlepage
title: Wi-Fi Security Review
---
# Wi-Fi Security Survey

This experiment is part of a research project at KU Leuven supervised by Prof. Mathy Vanhoef. The project aims to test how many networks are still vulnerable to the [FragAttacks](https://www.fragattacks.com) vulnerabilities. These vulnerabilities were discovered in 2020 and were publicly disclosed in 2021 after a 9-month embargo period, giving vendors an (exceptionally) long time to prepare and distribute security updates. This experiment investigates how many networks have, by now, still not received or installed security updates and are therefore still vulnerable.

A tool was created to test Wi-Fi networks automatically. This tool interacts with Wi-Fi networks to test them for various properties, and the results of these tests are then used to infer whether the network is (likely) vulnerable. During some of these interactions with the network, the tool will send open authentication and association frames, but will not perform any cryptographic handshakes to attempt to login on to the network. In other words, the tool does not try to guess passwords and does not try to gain access to the network. Instead, it sends a limited number of Wi-Fi frames and inspects the network's reaction. This also means no actual attack is performed or simulated against the network. Any data obtained from this experiment will be anonymized.

Our tests can be detected by the string `This is a test, see survey.fragattacks.com` that is included in several packets sent during the tests. Our survey is being conducted between February and March 2025 in Belgium and was previously also conducted around Leuven (Belgium) from March to June 2023. You can exclude your network from our tests by adding [`_nomap`](https://support.google.com/maps/answer/1725632?hl=en) or [`_optout`](https://social.technet.microsoft.com/wiki/contents/articles/32109.disabling-wifi-sense-by-gui-and-gpo-script.aspx) to the network name.

If you have any questions or remarks about this experiment, or you want your network to be excluded from future tests, you can contact us by sending an e-mail to mathy.vanhoef@kuleuven.be
