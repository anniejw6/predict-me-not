# predict-me-not

A web application to allow friends to make predictions about each other

One places bets in the format of "I bet that this event [does/does not] happen. I would risk [XX] credits to gain 100 credits if this event [does/does not happen]."

* Django webapp
* Facebook authentication

# Model Structure
* Proposal
  * proposal_id
  * side (happens/does not happen)
  * amount
  * time
* Bid (Succesful proposal)
  * bid_id
  * bet_id
  * positive_proposal_id
  * negative_proposal_id
  * actual_odds
  * time
* Bet
  * bet_id
  * Topic
  * Subject (the person the bet is about)
  * Date
  * Verifier

# Privacy
* In order to place or view bets, you must opt-in to having bets made about you
* Can only view bets of your friends
