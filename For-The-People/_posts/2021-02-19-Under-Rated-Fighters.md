---
category: arts
---

 <br>

Introduction
------------

In other posts, we’ve explored [how to understand fight
odds](https://aggression-to-the-mean.github.io/AttM/for-the-people/arts/2021/02/16/Understanding-Fight-Odds.html)
and described the [accuracy of UFC fight
odds](https://aggression-to-the-mean.github.io/AttM/for-the-people/arts/2021/02/16/How-Accurate-are-Fight-Odds.html).
It is natural to then wonder how well the fight odds have predicted the
performance of particular fighters.

The purpose of this post is to identify some of the most Under Rated
fighters in the UFC.

<br>

Defining “Under Rated”
======================

Before we can address the above question, it is critical that we define
some key terms. For starters, what does it mean for a fighter to be
Under Rated? To answer that question, let’s recall how we assessed the
overall accuracy of the odds: we examined if the favorites (or
underdogs) won at a rate similar to what would have been expected by the
Implied Probability of their odds.

We can use a similar logic to assess the Over Performance of particular
fighters. If a fighter wins at a greater rate than the average Implied
Probability of their odds, then they are overperforming relative to the
odds. If a fighter is overperforming, then they have been Under Rated by
the odds.

<br>

Dataset - Historical Data of UFC Fight Odds
===========================================

Using data science tools such as web scraping, I have obtained a dataset
with fight odds information regarding the majority of the UFC fights
that occurred between 2013 and present.

In particular, the dataset consists of 2941 UFC fights from 261 UFC
events, spanning from April 27, 2013 to February 06, 2021.

Among other things, the dataset lists the best odds for each fighter
around the time of their fight, as well as the winner of each fight.

<br>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>NOTE:</strong> Some of the tables below are based on the fight data contained in the dataset described above. Although the dataset captures a large proportion of UFC events and fights since 2013, it is not exhaustive. Therefore, I will do manual searches to retrieve additional data regarding the fighters in question, to provide a more comprehensive picture this fighter-specific odds information.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<br>

Under Rated Fighters
--------------------

The below table lists the top 10 Under Rated fighters, in the dataset,
with at least 5 UFC fights. These fighters are listed in order of Over
Performance, which is simply the Actual Rate of Victory subtracted by
Average Adjusted Implied Probabilities of the odds.

<br>

<table>
<caption>Top 10 Under Rated Fighters with at least 5 Fights</caption>
<colgroup>
<col style="width: 17%" />
<col style="width: 13%" />
<col style="width: 32%" />
<col style="width: 21%" />
<col style="width: 16%" />
</colgroup>
<thead>
<tr class="header">
<th style="text-align: left;">Fighter Name</th>
<th style="text-align: right;">Number of Fights</th>
<th style="text-align: right;">Average Adjusted Implied Probability (%)</th>
<th style="text-align: right;">Actual Rate of Victory (%)</th>
<th style="text-align: right;">Over Performance (%)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Leonardo Santos</td>
<td style="text-align: right;">5</td>
<td style="text-align: right;">45</td>
<td style="text-align: right;">100</td>
<td style="text-align: right;">55</td>
</tr>
<tr class="even">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: right;">10</td>
<td style="text-align: right;">50</td>
<td style="text-align: right;">100</td>
<td style="text-align: right;">50</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Brandon Moreno</td>
<td style="text-align: right;">7</td>
<td style="text-align: right;">44</td>
<td style="text-align: right;">86</td>
<td style="text-align: right;">42</td>
</tr>
<tr class="even">
<td style="text-align: left;">Arnold Allen</td>
<td style="text-align: right;">6</td>
<td style="text-align: right;">59</td>
<td style="text-align: right;">100</td>
<td style="text-align: right;">41</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Brian Ortega</td>
<td style="text-align: right;">8</td>
<td style="text-align: right;">48</td>
<td style="text-align: right;">88</td>
<td style="text-align: right;">40</td>
</tr>
<tr class="even">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: right;">8</td>
<td style="text-align: right;">61</td>
<td style="text-align: right;">100</td>
<td style="text-align: right;">39</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Bryan Caraway</td>
<td style="text-align: right;">5</td>
<td style="text-align: right;">42</td>
<td style="text-align: right;">80</td>
<td style="text-align: right;">38</td>
</tr>
<tr class="even">
<td style="text-align: left;">Yan Xiaonan</td>
<td style="text-align: right;">5</td>
<td style="text-align: right;">62</td>
<td style="text-align: right;">100</td>
<td style="text-align: right;">38</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Amanda Nunes</td>
<td style="text-align: right;">12</td>
<td style="text-align: right;">55</td>
<td style="text-align: right;">92</td>
<td style="text-align: right;">37</td>
</tr>
<tr class="even">
<td style="text-align: left;">Germaine de Randamie</td>
<td style="text-align: right;">8</td>
<td style="text-align: right;">53</td>
<td style="text-align: right;">88</td>
<td style="text-align: right;">35</td>
</tr>
</tbody>
</table>

<br>

Since the dataset is not exhaustive, I will guide you through some
additional, manual checks to get a more comprehensive overview of a
particular fighter’s relationship with the odds.

The odds in the dataset are derived from the [BetMMA.tips
website](https://www.betmma.tips/). However, for the manual checks, we
will query the [BestFightOdds website](https://www.bestfightodds.com/)
for the missing odds information. The best fight odds acquired from
these two sources should be sufficiently similar for our purposes.

We will also verify a fighter’s UFC history via the \[UFC’s site\]
(<a href="https://www.ufc.com/athletes/all/active" class="uri">https://www.ufc.com/athletes/all/active</a>).

<br>

Leonardo Santos
===============

The below table displays the Leonardo Santos fights that are included in
the dataset.

<br>

<table>
<caption>Leonardo Santos Fights Included in the Dataset</caption>
<thead>
<tr class="header">
<th style="text-align: left;">Fighter Name</th>
<th style="text-align: left;">Event</th>
<th style="text-align: left;">Date</th>
<th style="text-align: left;">Result</th>
<th style="text-align: right;">Adjusted Implied Probability (%)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Leonardo Santos</td>
<td style="text-align: left;">UFC Fight Night: Bigfoot vs Arlovski</td>
<td style="text-align: left;">2014-09-13</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">68</td>
</tr>
<tr class="even">
<td style="text-align: left;">Leonardo Santos</td>
<td style="text-align: left;">UFC Fight Night: Maia vs LaFlare</td>
<td style="text-align: left;">2015-03-21</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">44</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Leonardo Santos</td>
<td style="text-align: left;">UFC 194: Aldo vs McGregor</td>
<td style="text-align: left;">2015-12-12</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">15</td>
</tr>
<tr class="even">
<td style="text-align: left;">Leonardo Santos</td>
<td style="text-align: left;">UFC 204: Bisping vs. Henderson</td>
<td style="text-align: left;">2016-10-08</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">35</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Leonardo Santos</td>
<td style="text-align: left;">UFC Fight Night: Gustafsson vs. Smith</td>
<td style="text-align: left;">2019-06-01</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">60</td>
</tr>
</tbody>
</table>

<br>

According to the UFC website, [Leonardo
Santos](https://www.ufc.com/athlete/leonardo-santos) also had the
following fights:

<table>
<thead>
<tr class="header">
<th style="text-align: left;">Date</th>
<th style="text-align: center;">Result</th>
<th style="text-align: right;">Opponent</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">2013-06-08</td>
<td style="text-align: center;">Winner</td>
<td style="text-align: right;">Macario</td>
</tr>
<tr class="even">
<td style="text-align: left;">2014-03-23</td>
<td style="text-align: center;">Majority Draw</td>
<td style="text-align: right;">Parke</td>
</tr>
</tbody>
</table>

<br>

The odds information regarding the Macario fight does not appear to be
available on
[BestFightOdds](https://www.bestfightodds.com/fighters/Leonardo-Santos-1213).
However, since Santos won, we will disregard that fight. We will also
ignore the draw (though Santos happened to be the underdog).

**Therefore, based on Santos’ last 5 fights, he has overperformed,
relative to the odds, by a whopping 55%. Put another way, the odds only
gave Santos a 1% probability of winning all 5 fights.**

<br>

Robert Whittaker
================

The below table displays the Robert Whittaker fights that are included
in the dataset.

<table>
<caption>Robert Whittaker Fights Included in the Dataset</caption>
<thead>
<tr class="header">
<th style="text-align: left;">Fighter Name</th>
<th style="text-align: left;">Event</th>
<th style="text-align: left;">Date</th>
<th style="text-align: left;">Result</th>
<th style="text-align: right;">Adjusted Implied Probability (%)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC 160: Velasquez vs Silva 2</td>
<td style="text-align: left;">2013-05-25</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">39</td>
</tr>
<tr class="even">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC Fight Night: Miocic vs Hunt</td>
<td style="text-align: left;">2015-05-09</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">44</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC 193: Rousey vs Holm</td>
<td style="text-align: left;">2015-11-14</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">42</td>
</tr>
<tr class="even">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC 197: Jones vs Saint Preux</td>
<td style="text-align: left;">2016-04-23</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">74</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC Fight Night: Whittaker vs. Brunson</td>
<td style="text-align: left;">2016-11-26</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">44</td>
</tr>
<tr class="even">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC on FOX: Johnson vs. Reis</td>
<td style="text-align: left;">2017-04-15</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">29</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC 213: Romero vs. Whittaker</td>
<td style="text-align: left;">2017-07-08</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">52</td>
</tr>
<tr class="even">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC 225: Whittaker vs. Romero 2</td>
<td style="text-align: left;">2018-06-09</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">72</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC Fight Night: Whittaker vs. Till</td>
<td style="text-align: left;">2020-07-25</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">55</td>
</tr>
<tr class="even">
<td style="text-align: left;">Robert Whittaker</td>
<td style="text-align: left;">UFC 254: Khabib vs. Gaethje</td>
<td style="text-align: left;">2020-10-24</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">49</td>
</tr>
</tbody>
</table>

<br>

According to the UFC website, [Robert
Whittaker](https://www.ufc.com/athlete/robert-whittaker) also had the
following fights (odds retrieved from
[BestFightOdds](https://www.bestfightodds.com/fighters/Robert-Whittaker-3761#)):

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 15%" />
<col style="width: 16%" />
<col style="width: 18%" />
<col style="width: 18%" />
<col style="width: 13%" />
</colgroup>
<thead>
<tr class="header">
<th style="text-align: left;">Date</th>
<th style="text-align: center;">Result</th>
<th style="text-align: center;">Decimal Odds</th>
<th style="text-align: center;">Opponent Decimal Odds</th>
<th style="text-align: center;">Adjusted Implied Probability (%)</th>
<th style="text-align: right;">Over Performance (%)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">2012-12-14</td>
<td style="text-align: center;">Winner</td>
<td style="text-align: center;">1.43</td>
<td style="text-align: center;">3.25</td>
<td style="text-align: center;">70</td>
<td style="text-align: right;">30</td>
</tr>
<tr class="even">
<td style="text-align: left;">2013-08-28</td>
<td style="text-align: center;">Loser</td>
<td style="text-align: center;">1.63</td>
<td style="text-align: center;">2.70</td>
<td style="text-align: center;">62</td>
<td style="text-align: right;"><strong>-</strong>62</td>
</tr>
<tr class="odd">
<td style="text-align: left;">2014-02-22</td>
<td style="text-align: center;">Loser</td>
<td style="text-align: center;">2.22</td>
<td style="text-align: center;">1.77</td>
<td style="text-align: center;">44</td>
<td style="text-align: right;"><strong>-</strong>44</td>
</tr>
<tr class="even">
<td style="text-align: left;">2014-06-28</td>
<td style="text-align: center;">Winner</td>
<td style="text-align: center;">1.41</td>
<td style="text-align: center;">3.30</td>
<td style="text-align: center;">70</td>
<td style="text-align: right;">30</td>
</tr>
<tr class="odd">
<td style="text-align: left;">2014-11-07</td>
<td style="text-align: center;">Winner</td>
<td style="text-align: center;">2.71</td>
<td style="text-align: center;">1.54</td>
<td style="text-align: center;">36</td>
<td style="text-align: right;">64</td>
</tr>
<tr class="even">
<td style="text-align: left;">2019-10-05</td>
<td style="text-align: center;">Loser</td>
<td style="text-align: center;">2.20</td>
<td style="text-align: center;">1.90</td>
<td style="text-align: center;">46</td>
<td style="text-align: right;"><strong>-</strong>46</td>
</tr>
</tbody>
</table>

<br>

By taking a weighted average of (i) the average Over Performance for the
6 fights above (i.e. -4.7%) and (ii) the average Over Performance of the
10 fights in the dataset (i.e. 50%), we come to about 29%.

**Therefore, in Whittaker’s 16 fight UFC career, he has overperformed,
relative to the odds, by about 29%.**

<br>

Alexander Volkanovski
=====================

The below table displays the Alexander Volkanovski Fights fights that
are included in the dataset.

<table>
<caption>Alexander Volkanovski Fights Included in the Dataset</caption>
<colgroup>
<col style="width: 19%" />
<col style="width: 34%" />
<col style="width: 9%" />
<col style="width: 6%" />
<col style="width: 29%" />
</colgroup>
<thead>
<tr class="header">
<th style="text-align: left;">Fighter Name</th>
<th style="text-align: left;">Event</th>
<th style="text-align: left;">Date</th>
<th style="text-align: left;">Result</th>
<th style="text-align: right;">Adjusted Implied Probability (%)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC Fight Night: Whittaker vs. Brunson</td>
<td style="text-align: left;">2016-11-26</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">63</td>
</tr>
<tr class="even">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC Fight Night: Lewis vs. Hunt</td>
<td style="text-align: left;">2017-06-10</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">82</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC Fight Night: Werdum vs. Tybura</td>
<td style="text-align: left;">2017-11-18</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">85</td>
</tr>
<tr class="even">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC 221: Romero vs. Rockhold</td>
<td style="text-align: left;">2018-02-10</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">61</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC Fight Night: Dos Santos vs. Ivanov</td>
<td style="text-align: left;">2018-07-14</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">68</td>
</tr>
<tr class="even">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC 232: Jones vs. Gustafsson 2</td>
<td style="text-align: left;">2018-12-29</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">44</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC 237: Namajunas vs. Andrade</td>
<td style="text-align: left;">2019-05-11</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">44</td>
</tr>
<tr class="even">
<td style="text-align: left;">Alexander Volkanovski</td>
<td style="text-align: left;">UFC 245: Usman vs. Covington</td>
<td style="text-align: left;">2019-12-14</td>
<td style="text-align: left;">Winner</td>
<td style="text-align: right;">41</td>
</tr>
</tbody>
</table>

<br>

According to the UFC website, [Alexander
Volkanovski](https://www.ufc.com/athlete/alexander-volkanovski) also had
the following fights (odds retrieved from
[BestFightOdds](https://www.bestfightodds.com/fighters/Alexander-Volkanovski-9523):

<table>
<colgroup>
<col style="width: 17%" />
<col style="width: 15%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 19%" />
<col style="width: 14%" />
</colgroup>
<thead>
<tr class="header">
<th style="text-align: left;">Date</th>
<th style="text-align: center;">Result</th>
<th style="text-align: center;">Decimal Odds</th>
<th style="text-align: center;">Opponent Decimal Odds</th>
<th style="text-align: center;">Adjusted Implied Probability (%)</th>
<th style="text-align: right;">Over Performance (%)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">2020-07-11</td>
<td style="text-align: center;">Winner</td>
<td style="text-align: center;">1.53</td>
<td style="text-align: center;">2.96</td>
<td style="text-align: center;">66</td>
<td style="text-align: right;">34</td>
</tr>
</tbody>
</table>

<br>

By taking a weighted average of (i) the average Over Performance for the
one fight above (i.e. 34%) and (ii) the average Over Performance of the
8 fights in the dataset (i.e. 40%), we come to about 39%.

**Therefore, in Volkanovki’s 9 fight UFC career, he has overperformed,
relative to the odds, by a staggering 39%.**

<br>

Conclusion
----------

In this post, I identified a few of the most Under Rated fighters on the
UFC roster. By doing the same manual checks as I did, you could go down
the list of the top 10 overperformers from the dataset and calculate the
actual UFC Over Performance stats for the fighters not covered in this
post.
