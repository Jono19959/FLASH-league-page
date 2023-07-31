<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;
    let participants;
    let financials;
    let auctionRules;
    let tradeRules;
    let waiverWireSystem;
    let rosterManagement;
    let scoring;
    let scheduling;
    let lastPlacePunishment;
    let pressConferences, weeklyPressConferences, yearlyPressConferences;
    let ruleChanges;
    let codeOfConduct;
    let lastNote;
    

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">FLASH Manifesto</h1>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(participants)}>Participants</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(financials)}>Financials</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(auctionRules)}>Auction Rules</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(tradeRules)}>Trade Rules</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(waiverWireSystem)}>Waiver Wire System</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(rosterManagement)}>Roster Management</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(scoring)}>Scoring</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(scheduling)}>Regular Season/Playoff Scheduling</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(lastPlacePunishment)}>Last Place Punishment</h3>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(pressConferences)}>Press Conferences</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(weeklyPressConferences)}>Weekly Press Conferences</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(yearlyPressConferences)}>End-of-Year Press Conferences</h4>
 
    <h3 class="noUnderscore clickable" on:click={() => goToSection(ruleChanges)}>Rule Additions and Modifications</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(codeOfConduct)}>Code of Conduct</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(lastNote)}>Note From the Commissioner</h3>   
  
    
    <hr />
    
    <h3 class="sectionHeading" bind:this={participants}>Participants</h3>

    <ol>
        <li>Chris Keane</li>
        <li>Dominic Martinez</li>
        <li>Ethan Fortin <mark>/ Casey Vaughn</mark></li>
        <li>Jacob Mayer</li>
        <li>Jeremy Vilchez</li>
        <li>Joe Donovan</li>
        <li>Jonathan Collins</li>
        <li>Luke Natalo</li>
        <li>Matt Kolln</li>
        <li>Peter Psyllos</li>
        <li>Ryan Cullen</li>
        <li>Ryan Vaughn</li>
    </ol>

    <h3 class="sectionHeading" bind:this={financials}>Financials</h3>

    <b>Total Payment: $50</b><br>
    <ul>
        <li>Entry Fee: <b>$50</b></li>
    </ul>
    
    All payments must be paid directly to the commissioner by the time the auction draft starts.<br><br>
    <b>Total (starting) Prize Pool = $600</b><br>
    <b>End-of-Season Payouts:</b><br>
    <ul>
        <li>First place: <b>$360</b> (60%)</li>
        <li>Second place: <b>$180</b> (30%)</li>
        <li>Regular season highest scorer: (based on points scored with record as the tiebreakers): <b>$60</b> (10%)</li>
    </ul>
    
    <h3 class="sectionHeading" bind:this={auctionRules}>Auction Rules</h3>

    <ol>
        <li>Teams will be drafted via a live auction. If a GM is not able to attend the live auction they may designate a stand-in to draft for them.</li>
        <li>Teams have a budget of $200</li>
        <li>The nomination order will the reverse standings of the previous year</li>
        <li>
            Teams consist of 18 players:
            <ul>
                <li>QB</li>
                <li>2 RB's</li>
                <li>2 WR's</li>
                <li>TE</li>
                <li>2 Flex's*</li>
                <li>D/ST</li>
                <li>6 bench slots</li>
                <li>2 IR's^</li>
                <li>2 WR's</li>
            </ul>
            *Flex can be filled by RB, WR, or TE<br>
            ^IR slot can only be filled by players declared OUT (not SUSP)
        </li>
        <li>A team must draft a player to fill all 9 starting slots (i.e. a GM may not forgo drafting a TE or D/ST with intentions of picking one up off the waivers post draft)</li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={tradeRules}>Trade Rules</h3>

    <ol>
        <li>All GMs have the option to veto any accepted trade.  Trades will be processed 24 hours after the acceptance of a trade.</li>
        <li>By not voting, you are agreeing the trade is fair.</li>
        <li>In order to overturn a trade there must be 7 votes to veto (super majority of the 10 GMs not involved in the trade).</li>
        <li>The trade deadline is week 10.</li>
        <li>
            If you want a trade to forgo the normal veto process for any reason, the following steps must be taken
            <ol type="a">
                <li>(Optional) Post the trade in the groupme (specifying all details of the trade)</li>
                <li>Four other GMs not involved in the trade must approve the trade either by liking the groupme post or by voting "PASS" in Sleeper.</li>
                <li>Once you have approval from the league, DM Jodo and/or Jono (most likely Jodo) at least 2 hours before the start of the next round of NFL games (by 6:20pm EST Thursday or 11:00am EST Sunday) so that they can push the trade through.</li>
                <li>Either commissioner will send both GMs involved in the trade a confirmation when they push the trade through. So be ready to set your lineups.</li>
            </ol>
        </li>
        <li>Trading of your current season FAAB budget is allowed.</li>
        <li>Trading of your future auction budget for current players is not allowed.</li>
        <li>Off-season trades are allowed as long as all players involved are kept by both GMs and the vote is not vetoed by the league.</li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={waiverWireSystem}>Waiver Wire System</h3>

    <ol>
        <li>The waiver wire system will be FAAB (free agent acquisition budget)</li>
        <li>All GMs will start the season with a FAAB budget of $100 PLUS any money left over from the auction</li>
        <li>If available players go through their waiver period without being picked up, they will become free agents</li>
        <li>The minimum FAAB bid for a player is $0</li>
        <li>The tie-breaker for multiple people bidding the same amount for a player is reverse current standings</li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={rosterManagement}>Roster Management</h3>

    <ol>
        <li>
            Each team must field a full roster each week.  If a team fails to do so by the end of the week, the commissioner has the option to retroactively fill in the team roster with the lowest scoring eligible player.
            <ol type="a">
                <li>This does not apply if the GM intentionally leaves a slot empty or does not have a qualifying player to fill a slot (i.e. COVID-19 situations or no D/ST due to byes).</li>
            </ol>
        </li>
        <li>
            The team GM will be removed at the commissioner’s discretion if a full roster is not fielded 2 or more times in a given season.
            <ol type="a">
                <li>The vacant team will be managed by the commissioner until a replacement can be found unless the commissioner’s team plays the vacant team.  Then the current highest seeded team (other than the commissioner) will manage the team for that week.</li>
            </ol>
        </li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={scoring}>Scoring</h3>

    <ol>
        <li>Sleeper default options have been selected for our scoring system.</li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={scheduling}>Regular Season/Playoff Scheduling</h3>

    <ol>
        <li>The regular season will last 14 weeks</li>
        <li>
            The top six teams in the league will advance to the championship bracket
            <ol type="a">
                <li>The championship bracket will last 3 weeks, with the Championship occurring on week 17 of the NFL regular season</li>
                <li>The top team in each division will secure a bye for the first round, automatically advancing to the semi-finals</li>
            </ol>
        </li>
        <li>
            The bottom six teams in the league will play in the postseason Toilet Bowl
            <ol type="a">
                <li>The Toilet Bowl will last 3 weeks, with the finals occurring on week 17 of the NFL regular season</li>
                <li>The 2 worst teams will secure a bye for the first round, automatically advancing to the semi-finals</li>
                <li>The team that scores the least amount of points in each matchup is the team that advances to the next round</li>
            </ol>
        </li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={lastPlacePunishment}>Last Place Punishment</h3>

    <ol>
        <li>All GMs can collectively add ideas of potential punishments to a list prior to the start of the NFL regular season.</li>
        <li>The loser (GM with the least points scored in the final round) of the aforementioned Toilet Bowl will have to partake in a punishment of their choice from the list created by the league. They will have to send proof of completion of punishment to the league prior to the start of the following NFL preseason.</li>
        <li>Failure to complete punishment will result in a fine of $50 that will go towards food and drinks for the live draft next season.</li>
    </ol>
    
    <h3 class="sectionHeading" bind:this={pressConferences}>Press Conferences</h3>
    
    <h4 bind:this={weeklyPressConferences}><del>Weekly Press Conferences</del></h4>
    <div class="subBlock">
        <ol>
            <li><del>Every week in the regular season, the lowest scorer from that week must share a “press conference” answering any submitted questions from the rest of the league</del></li>
            <li>
                <del>Weekly press conference schedule is as follows</del>
                <ol type="a">
                    <li><del>Starting Tuesday morning, all non-losing GMs have until Wednesday noon EST to submit one question to Jodo to be delivered to the losing GM</del></li>
                    <li><del>Jodo will deliver those questions to the losing GM by midnight EST on Wednesday night</del></li>
                    <li><del>The losing GM has until Saturday @ 5:00pm EST to record themselves answering the questions andpost the “press conference” to either the groupMe channel or another publicly accessible location</del></li>
                </ol>
            </li>
            <li><del>Outside of managing their team, this is the only responsibility each GM potentially has on a week-to-week basis, but this is an expectation for being in this league. If you have any issues recording or posting your press conference, please reach out to Jodo or Jono</del></li>
        </ol>
    </div>

    <h4 bind:this={yearlyPressConferences}><del>End-of-Year Press Conferences</del></h4>
    <div class="subBlock">
        <ol>
            <li><del>At the conclusion of the regular season, each team who did not make the championship bracket will have to give an extended press conference, similar to the weekly press conference</del></li>
            <li>
                <del>These press conferences will start in week 14 of the NFL regular season and will last X amount of weeks, with 2 GMs going each week</del>
                <ol type="a">
                    <li><del>The schedule for the press conferences will be released shortly after the conclusion of the FLASH regular season (first teams eliminated from playoff contention will most likely go first)</del></li>
                </ol>
            </li>
            <li><del>All other GMs are allowed to submit 2 questions to Jodo or Jono for an eliminated GM by midnight EST on Wednesday night of the week the GM is to give their press conference</del></li>
            <li><del>The eliminated GM must post their press conference by Sunday @ 1:00pm EST</del></li>
            <li><del>There is a potential to have to answer 22 questions, so plan enough time before you start</del></li>
            <li><del>Failure to submit your press conference will result in a penalty of some sort (TBD)</del></li>
        </ol>
    </div>

    <h3 class="sectionHeading" bind:this={ruleChanges}>Rule Additions and Modifications</h3>

    <ol>
        <li>Any suggested modifications to any of the rules outlined above will be voted on by the entire league and must get a majority vote to make the modification to this document</li>
        <li>Any rules not stated above will be decided by the league through our GroupMe chat and will be added to this document as soon as possible</li>
        <li>
            The commissioner will only override potential rule additionals and modifications if it creates a lot more work for the commissioner.
            <ol type="a">
                <li>However, if a GM is willing to do the work for the rule change to go in effect, the commissioner will lose his or her ability to override any rule change</li>
            </ol>
        </li>
    </ol> 
    
    <h3 class="sectionHeading" bind:this={codeOfConduct}>Code of Conduct</h3>

    <p>Because we are a group of friends who just want to have fun playing fantasy football, there is not a “zero-tolerance” policy for any actions that are considered “harmful” to the group or an individual of this league. Everyone has come from a different backgrounds, so try to be respectful of everyone else’s beliefs. If you have any questions or concerns about how someone is acting, please reach out to the commissioner or talk to the individual about it before it has the potential to escalate into something bigger.</p>
    <p>If any issues get to a point where we can’t settle the issue civilly, the following steps will be taken:</p>
    <ol>    
        <li>A warning will be given to the instigator of the issue, and that behavior should stop immediately</li>
        <li>If that behavior continues, the commissioner will have the option of removing that individual from the league. A refund for the league will be determined on a case-by-case basis.</li>
    </ol>
  
    <h3 class="sectionHeading" bind:this={lastNote}>Note from the Commissioner</h3>

    <p>I will never ever ever take anything in this league as seriously as this article makes it seem. I just wanted a clearly defined set of rules written out now so that the rest of this season can be focused on interactive fantasy football fun. But if you’re deciding you don’t wanna play this year, feel free to use one of the rules above as a reason for leaving the league - don’t worry, I’ll completely understand.</p>
    
</div>
