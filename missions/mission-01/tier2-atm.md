## steps to dispense money to a customer via atm.
- customer inserts card
- try verifying the card
- if card cannot be read, return card and END with “Card could not be read.” response
- if the card is not a valid card or expired, don't return the person's card but return a "card is invalid or has expired" response and END
- if the card is valid then ask customer for pin
- customer enters pin
- try checking and verifying the pin
- if the pin is wrong: 
- return a "wrong pin, try again" response to the customer then go back to line 7 
- if a wrong pin repeats up to five times for the same card then return a "wrong pin after 5 attempts", keep the person's card and END
- if the pin is correct, ask the customer for the kind of transaction he or she wants to perform.
- the customer selects withdrawal
- ask the person the amount he or she wants to withdraw.
- the customer enters the amount
- check if the amount is less than 200 naira
- if the amount is less than 200 naira, return "cannot dispense amounts less than 200 naira" response, return the person's card and END
- try to check the available balance in the account that is attached to the card
- if the withdrawal amount is greater or equal to the available balance (this is because you cannot withdraw all the balance you have in an account, so withdrawal amount always has to be less than the available balance)
- return "insufficient funds" response, return the person's card and END
- if the amount is less than the available balance in the account attached to the card, (which makes it possible for the person to be able to withdraw)
- try verifying if there is enough money on the ATM at the moment to pay the customer
- if there is not enough money or currency notes on the atm at the moment, tell the customer that the atm cannot dispense that amount at the moment and return the person's card and END
- if there is enough money, try performing the withdrawal
- if there is an unknown error (server error, or maybe due to bad network that prevented the transaction from going through), return "transaction cannot be completed", response, return the person's card and END
- dispense the said amount to the person at once with a "take your money from the cash dispenser" response.
- update the available balance in the account that the card is attached to, return a "take your card" response, and END


## My reasoning section
### why i think each step is necessary in a paragraph
The computer is understood to be a dumb literal machine that does not and cannot guess like a human does when put to work, so in as much as it is good and easier when computers are given tasks to complete, the only possibility of such a task to be completed accurately depends on how well the computer system was informed of the data it is going to be working with while it completes the said task. so everything has to be exact, literal and accurate, else the computer would have to guess at some points which would lead to wrong results.
As for why i think its right to check for all edge cases, when designing systems and automating software, there is no guarantee that everything will go as smooth as it should, so as a good engineer, i need to design a software or automate a system that already takes into account of all possible errors or wrong input or information that my system could possibly be dealing with when it is put in the real world. 

### Here are my detailed points justifying why each step is necessary 
- The card is verified before asking for the PIN to make sure only valid ones are being worked with on the ATM. 
- The account is updated only when there is a successful withdrawal because it is the only point where the person's funds in the account that is attached to the card are touched or tampered with. this makes sure a person is not debited without the person actually dispensing money to the person 
- The card is kept after too many failed attempts because of security reasons, it would prevent the person from going to try the same card on another ATM as well. and it also ensures order for people to know that an expired card cannot and should not be used anymore.
- the balance is checked first before checking the ATM’s cash because it is only when one has a said withdrawal amount in the bank that he or she can withdraw from the account. so this helps to know if the withdrawal is viable or not
