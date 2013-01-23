#Card payment

## Package
The main Namespace is com.progress.demo.rce.card

## Events
* **NewTerminal**(integer id). It defines a new terminal that will receive the payments made by the simulator.
* **NewSim**(integer id). It defines a new payment simulator for the ID-terminal.
* **Pay**(integer id, integer card, float amount, string currency). Pay event that includes the terminal id where it was made, a random card number, a random amount and the pay currency.
* **Stream**(string channel, integer idChannel, integer idClient, sequence<string> extra). The output event that has the information about the channel, its id, the client id and the extra information.
In this case, the channel is "CARD", its id corresponds to the terminal number, the client id is defined by the card number, and extra = [amount, currency].