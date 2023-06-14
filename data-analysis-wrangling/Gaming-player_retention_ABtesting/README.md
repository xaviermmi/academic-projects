# Retention analysis over AB tests

## 1. Introduction
<p><a href="https://www.facebook.com/cookiecatsgame">Cookie Cats</a> is a hugely popular mobile puzzle game developed by <a href="http://tactile.dk">Tactile Entertainment</a>. It's a classic "connect three"-style puzzle game where the player must connect tiles of the same color to clear the board and win the level. It also features singing cats. We're not kidding! Check out this short demo:</p>
<p><a href="https://youtu.be/GaP5f0jVTWE"><img src="https://github.com/xaviermmi/academic-projects/assets/122324304/c92981f8-109f-45fa-9058-ba169f5737a9" style="width: 500px"></a></p>
<p>As players progress through the levels of the game, they will occasionally encounter gates that force them to wait a non-trivial amount of time or make an in-app purchase to progress. In addition to driving in-app purchases, these gates serve the important purpose of giving players an enforced break from playing the game, hopefully resulting in that the player's enjoyment of the game being increased and prolonged.</p>
<p><img src="https://github.com/xaviermmi/academic-projects/assets/122324304/a24f54a7-93a8-4ceb-a7ec-9ad20d34e931" alt></p>

## 2. Project instructions
We've seen the importance of the gates...
<p>But where should the gates be placed? 
Initially the first gate was placed at level 30, but in this notebook we're going to analyze an AB-test where we moved the first gate in Cookie Cats from level 30 to level 40. In particular, we will look at the impact on player retention at 1-day and 7-days.

## 3. Dataset
<p>The data we have is from 90,189 players that installed the game while the AB-test was running. The variables are:</p>
<ul>
<li><code>userid</code> - a unique number that identifies each player.</li>
<li><code>version</code> - whether the player was put in the control group (<code>gate_30</code> - a gate at level 30) or the group with the moved gate (<code>gate_40</code> - a gate at level 40).</li>
<li><code>sum_gamerounds</code> - the number of game rounds played by the player during the first 14 days after install.</li>
<li><code>retention_1</code> - did the player come back and play <strong>1 day</strong> after installing?</li>
<li><code>retention_7</code> - did the player come back and play <strong>7 days</strong> after installing?</li>
</ul>
<p>When a player installed the game, he or she was randomly assigned to either <code>gate_30</code> or <code>gate_40</code>. As a sanity check, let's see if there are roughly the same number of players in each AB group. </p>

## 3. Skills
This project is showcasing basic marketing metric on app design alternatives : we are talking about retention rates measuring within AB-testing.
In terms of code, we use :
<li><code>pandas</code> for data manipulation skills and boostrapping techniques :
    <ul>> the aim is to build confidence in segmentation by enlarging the dataset</ul>
<li>simply<code>matplotlib</code> as plotting library
</li>

## 4. Project summary
The project notebook is organized in 6 parts :
<li>Import library & load data
<li>Distribution of game rounds
<li>1-day retention analysis and bootstrapping
<li>Statistical probability of a difference between gate 30 and gate 40
<li>7-days retention boostrapping and statistics
<li>Conclusion
</li>
