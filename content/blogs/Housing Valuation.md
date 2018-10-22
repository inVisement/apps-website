
---
title: "US Housing Valuation"
date: 2018-10-20
tags: ["Housing", "Valuation", "Chart", "yap", "yap-map", "Intrinsic Value"]
card:
    Are you undecided in buying or renting?
    Our interactive map helps you to find out if buying a home in your neighborhood is a good investment.
    <button class="readmorebtn">Read more</button>
---

<div id="more-text" style="display: none;">{{% inner-md %}}

### What does this map and app show?
How much will you gain if you buy a home instead of renting it. The total investment return for each US county.

### Why are some counties empty?
There was not enough relaible data to calculate the intrinsic economic value of properties in that county.

### What are the shortcomings?
Some counties are empty (Dah!) and we have not taken into account (yet) the homeowner insurance differences.
As soon as we find a reliable data source, we will improve it.

### What is this app NOT about?
There are many factors when you are deciding to buy a home. Are you settled in your job and town?
Can you afford the down-payment and mortgage payments? Do you like the freedom of moving or the pleasure of working on your home?
What type of housing do you like? What neighborhood is the right one for you?
These decision factors depend on personal preferences and we do not deal with them.

### Then, what the hell are you good for?
Buying a home means commiting to a long term investment, putting a good chunck of your savings for a down payment,
borrowing a huge amount of mortgage, and often paying twice in
"mortgage payment, property tax, rennovation costs, and homeowner insurance" as you might pay to rent a similar apartment or home.

But if you buy a home, you will profit from price appreciation, you avoid paying ever-increasing rents, and it can be a good retirement investment when you are done with mortgage payments.

Moreover, timing is another crucial factor. Maybe housing prices in your town have gone too high, or mortgage rates are too high to justify buying a home. Is it better to buy or to rent and wait?

We deal with all these "economic and financial" factors and make it simple for you. inVisement answers "is it a good investment?"

### Is it reliable? You know prediction is a fool's errand, right?
Nobody knows the future, but we stick to **economics of housing valuation**.
We use financial market rates to hedge risks and we avoid predicting as much we can.
We do not like to look like a fool.
We deploy Economics, Asset Pricing, Financial Market, Data Science, and Machine Learning to build, train, and test our valuation model.

### How do you do that?
We use "Economics and Asset Pricing" to come up with a reliable formula with a solid foundation to calculate
the intrinsic economic value of real estate properties.

Then, we use "Financial Market and Macroeconomic Indicators" to hedge all the hedgeable risks in order to avoid "predicting" and making a fool out of ourselves.

But not everything is hedge-able. So, we train our Machine Learning model to optimize the model accuracy. And, we use the most reliable and up-to-date data sources (thanks to our data providers: Zillow, Federal Reserve, our Municipal Tax Data and Insurance Data) to come up with our housing valuations for each neighborhood. At the end, we visualize it for you and keep it updated every week with new upcoming data. It's all we do. Simple. Would you like to do it on

your own?

### What if I trust you and lose money?
You are responsible for your investment decisions. Do not blame it on us. No kidding. It's legal.

### Can I distribute or use it?
Yes, it is free, we appreciate if you do so and we claim nothing on your gain without the pain.

<!--

### If you are not a fool (and neither am I), why is it free?
Do not worry about us making money. Really! You know, ad, premium account, connecting to sellers, omg, so many ways to make money in Freemium world.

### We are first time home shoppers? How are you going to help us?
Use "Total Gain in %" indicator. It says you how much you save or gain if you buy home in that neighborhood and keep it. (considering time value of money and many other financial factors).

### I am between: buying a home or renting and investing in stock market?
Use "Annual Return in %" and see if it exceeds your expectation from stock market return. For stock market analysis, you can use other inVisement tools. Also, remember risk and liquidiy are different for these two investment classes.

### Can I suggest a new feature or contact with you?
Definitely. Gracefully. Shoot us an email: invisement at gmail.

### How can I have your chart in my website/weblog?
Copy this code:

### I'd like be called a landlord by tenants.
Use ... and do not forget the costs and fees that are needed to manage properties an
I am a real estate investor and would like to buy and rent it and make good easy money.


### I am one of those 1% Americans. I can buy it all in cash.
Use ... and do not forget to diversify.

-->

{{% /inner-md %}}</div>



<b class="yap-caption"> Buy or Rent a home? </b>
<div id="yap-canvas">
    <b class="center">% Investment Return if you buy a home </b>
    <div id="yap-legend" class="right bottom"> % Annual Net Return: &nbsp </div>
</div>
<figure id="info-table" class="yap-canvas" style="width: 250px; position: relative">
</figure>

<link rel="stylesheet" type="text/css" href="http://127.0.0.1:8887/cdn/housing map.css"/>

<!--
<script src="http://127.0.0.1:8887/cdn/jquery-3.3.1.min.js"> </script>
-->

<script src="http://127.0.0.1:8887/cdn/housing map.js"></script>

<script>
    const moreText = "Read more";
    const lessText = "Read less";
    const moreButton = $("button.readmorebtn");
    moreButton.click(function() {
        const $this = $(this);
        $this.text($this.text() == moreText ? lessText : moreText)
        $("#more-text").toggle();
    });
</script>


