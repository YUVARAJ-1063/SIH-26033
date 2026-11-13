# Smart India Hackathon Workshop
# Date: 13/11/2026
## Reference Number: 26012582
## Name: YUVARAJ C

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
1. Detailed explanation of the proposed solution:

FARMER BELEIF is a toll-free phone number that any farmer can call from a basic keypad phone. A voice system speaks to the farmer in their own language (Tamil, Hindi, Telugu, etc.), tells them the price, and connects them to buyers.

2. How it addresses the problem:
```
  -->The farmer dials 1818 and speaks: crop name, quantity, and when it will be ready.
  -->The system tells the farmer today’s mandi price for that crop and the best nearby market or buyer, after subtracting transport cost.
  -->The produce is shown to registered buyers (traders, hotels, hostels, food companies, retailers). Buyers send their offers.
  -->The farmer hears the best offers on the next call or gets them as an SMS, and presses a key to accept one.
  -->A nearby village collection point (run by an FPO or Self-Help Group) weighs the produce, checks quality, and arranges pickup.
 -->Payment goes directly to the farmer’s bank account, and the farmer gets a confirmation SMS.
```
   
3. Innovation and uniqueness of the solution:
```
-->The farmer gets the real price without going through an agent.
-->Buyers compete for the produce, so the price goes up.
-->Every farmer, even one without a smartphone or education, can take part.
-->The collection point removes the need for the farmer to travel to the mandi.
```

## Technical Approach

1. Technologies to be used (e.g. programming languages, frameworks, hardware):
 ```
  --> Call system (IVR): Exotel / Twilio / Knowlarity toll-free number
  --> Speech recognition and voice replies: Bhashini (Government of India) or Google Speech-to-Text and Text-to-Speech
  --> Backend: Python (Flask or Django) or Node.js
  --> Database: PostgreSQL
  --> Price data: Agmarknet and eNAM open data
  --> Buyer side: a simple dashboard for buyers to view stock and send offers, used by the buyer only, not the farmer
  --> Payments: UPI / direct bank transfer through Razorpay
  --> SMS alerts: Twilio or MSG91
  --> Farmer records: mobile number linked with name, village, crop and bank details
```
  
3. Methodology and process for implementation <b>(Flow Charts/Images/ working prototype)</b>
```
          Farmer dials 1818 (toll-free)
                      |
                      v
       Voice system greets in the farmer's
        language and asks for crop details
                      |
                      v
      Farmer says: crop, quantity, ready date
                      |
                      v
      System converts speech to text and
           saves the listing
                      |
                      v
      System tells farmer today's price and
       best nearby market / buyer
                      |
                      v
       Listing is sent to registered buyers
                      |
                      v
         Buyers send their price offers
                      |
                      v
       Is the offer fair compared to the
             mandi price?
              /                \
            No                 Yes
            |                   |
            v                   v
     Offer is marked      Best offers sent to
     low and buyer is     farmer by call / SMS
     asked to revise              |
                                  v
                       Farmer presses a key to accept
                                  |
                                  v
                Village collection point weighs and
                 checks quality, pickup is arranged
                                  |
                                  v
                        Quality okay?
                       /            \
                     No             Yes
                     |               |
                     v               v
             Price adjusted     Payment sent to farmer's
             or dispute goes    bank account, SMS sent
             to FPO helper
```

## Feasibility and Viability

1. Analysis of the feasibility of the idea:
```
==>  Technical: Toll-free calling services, speech recognition and SMS are available from ready-made providers. Bhashini supports many Indian languages, and Agmarknet price data is free.
==>  Operational: India has a very large number of mobile phone users, including in villages, and farmers are already used to calling for information (like the Kisan Call Centre). Village FPOs and Self-Help Groups can run the collection points.
==>  Economic: There is no need to build an app or ask farmers to buy anything. The main costs are call charges and collection point staff. The platform earns a small commission of about 2 to 3% from buyers on completed sales, which is far lower than the margin the agents take.
==>  Starting plan: Begin with one district, one or two crops, a few collection points and a small group of buyers. Expand after the pilot
```
2. Potential challenges and risks:
```
--> The voice system may not understand different accents and local words.
-->  Farmers may not trust a phone system with their produce and money.
--> Not enough buyers may join in the beginning.
--> Poor mobile network in some villages.
--> Quality may be disputed at the collection point.
--> Running the collection points and transport costs money.
```

4. Strategies for overcoming these challenges:
```
 ==>  Accent problems: Train the system with local language samples, keep questions short and simple, and offer key-press options (like “press 1 for tomato”). If the system doesn’t understand, the call goes to a human helper.
 ==> Trust: Work through local FPOs and SHGs that farmers already know, send an SMS confirmation after every step, and start with a small pilot to show the first successful payments.
==> Few buyers: Start with hotels, hostels, canteens and food companies that already buy in bulk, and promise them regular supply and quality.
==> Poor network: The service works on ordinary calls and SMS, so it doesn’t need the internet. Farmers can call again later if the call drops, and the system saves the progress.
```

## Impact and Benefits:
1. Potential impact on the target audience:
```
==> Farmers: Fair price information, direct buyers, and no need for a smartphone or reading skill. Small and marginal farmers benefit the most.
==> Buyers: Regular supply of produce straight from the farm at a lower cost.
==> Village youth and SHGs: Jobs and income from running the collection points.
```

2. Benefits of the solution (social, economic, environmental, etc.):
```
==> Economic: Farmers earn more, and buyers spend less than they do through several middlemen.
==> Social: Includes farmers who are usually left out of digital solutions, including women and elderly farmers, and reduces dependence on agents and moneylenders.
==> Environmental: Selling at the right time to the right buyer reduces wasted produce, and joint pickup reduces the number of transport trips.
```

## Research and References
1. Details / Links of the reference and research work:
```
==> Agmarknet and eNAM websites for mandi prices
==> Kisan Call Centre (Ministry of Agriculture and Farmers Welfare) for the toll-free farmer helpline model
==>Bhashini (Government of India) for Indian language speech technology
Ministry of Agriculture and Farmers Welfare
```
