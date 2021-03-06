## NOTE - 11 MAR 18

TO INSTALL MY PACKAGE:

devtools::install_github("slackliner33/Yahoo_DFS_Optimizer/YahooDFSOptimizer")

(OR RUN:

devtools::install_github("slackliner33/Yahoo_DFS_Optimizer/YahooDFSOptimizer", quick=TRUE)

IF ANY TROUBLES ARISE WITH THE INSTALLATION)


THE PACKAGE IS SIMPLE...

ONLY 2 FUNCTIONS NEED TO BE RUN (IN ORDER) TO REACH END GOAL:

1. scrapeDFS()

- No arguments needed, produces data frame of scraped table (reduced) data

2. generateLineups()

- Also no arguments, produces data frame with 10 best (optimal) lineups for given NBA daily slate of games

While the functionality is simple, the 2 functions are running quite a bit of code to scrape player data, clean and sort it, prep a binary IP, solve it 10 times, and then produce user-friendly results.

If issues arise, note that this package requires the installation of "rvest" and "lpSolve"


# Yahoo_DFS_Optimizer - JAN 18
Tool to generate optimal line-ups for Yahoo DFS NBA Contests

1.1 

The proposed name for my tool will be called Yahoo_DFS_Optimizer.

1.2

This tool will allow the user to build optimal NBA line-ups for Yahoo’s Daily Fantasy contests. This tool will import data (scrape) from Yahoo’s site and then allow the user to adjust parameters as well as his/her projections while generating top line-ups. This tool will not work for NFL contests as the season is nearly over.

1.3

This tool will be useful to Yahoo NBA Daily Fantasy users because without their own software/scripts or an expensive subscription to an optimizer website, it is difficult for the average user to create optimal line-ups quickly and efficiently. This tool will provide a means for the average user to examine optimal line-ups without having to conduct all the monotonous and tedious work of copying, pasting, formatting, and running Solver in Excel to create line-ups.

1.3.A

This tool will be fairly rudimentary compared to many of the expensive subscription-based optimizer websites that are on the market currently. Once complete, this tool will provide the user with the five best line-ups according to his/her projections (and the scraped salary costs of the NBA players on any given contest day). Additionally, the tool will afford the opportunity for the user the lock in certain players or exclude others. In the end, this will save the average user tons of time, by quickly giving them the optimal predicted line-ups (based on his/her projections) that then he/she can input into Yahoo contests.

1.3.B

This optimizer tool will be a beneficial tool for the average daily fantasy player. This is a player who risks less than $50 a week. This implies that the player is on a budget or not into gambling lots of money. Thus, such a player is unlikely to pay $30+ a month to a subscription website, which means this tool could be very valuable for such a user, as he/she will likely have no other means of quickly generating optimal line-ups. To reiterate, this tool would not be used by fantasy experts (sharks) or those who are serious enough to have subscriptions to better websites/tools already. Furthermore, this tool would not be used by the occasional player who is in the contests more for gambling and less concerned with making his/her own projections and generating optimal line-ups.

1.3.C

A user of this tool would need computer/internet access, R, and Devtools. Additionally, he/she would need to have access to MS Excel (or another compatible program) so that he/she can create projections for the players. This tool will not create its own projections (like most subscription sites do) as that is extremely complicated to do well. Consequently, the user will have to have the means to use intuition, his/her own program, or the projections from a free website in order to be able to use the optimizer tool. This tool will require importation of files and some (minimal) understanding of how integer programming works. As this optimizer tool will run a binary integer program, it is important that the user understand minimally what is going on in the background.

1.3.D

This tool, as stated, will run via a binary integer program that uses the user’s own projections (for the players’ fantasy scores), the salary levels for each player according to Yahoo, and the requirements of the contests themselves to generate the five best line-ups.

1.3.E

This tool may involve some methodology or coding from the R package ffanalytics.

1.4

Users will be able to access this tool from the internet as a Shiny app.

1.5

None

1.6

None, no security concerns


---------------------------------

                   Feature                 Description                                                                         
    Scrape Yahoo!'s salary data      The ability to import the salaries for each player in the daily NBA contest 

    Import the user's projections    Will allow the user to upload his scoring projections for each player               

    Run the Optimizer 5 lineups      Binary integer program that takes inputs and generates 5 top line-ups           


---------------------------------

    Priority     Status                   Value
      1        Not started          Saves the user from having to manually look for and type them in him/herself

      2        Not started          Allows the user to have control over the projections that the model will use to create top line-ups

      3        Not started          Saves the user from having to guess & check or use Solver to make 5 optimal line-ups 


--------------------------------

                User.input                                                      Output  
    Potential option for user to pick which slate of NBA games       A list of players and their daily Yahoo salaries

    Must upload projections in a .txt, .csv, or .xlsx file (TBD)     A list of the players and their score projections

    None, except the user clicking "RUN" to start the optimizer      A list of the 5 top line-ups for the NBA contest

   ---------------------------
   
                                             Use.of.output

    users can examine this output as they could on the site, but it will be sortable this way and can help them build their projections

    The user can verify they made the right projections for the right players, and can manually adjust them in the tool if need be
    
    Allows the user to examine the five best line-ups and take the one(s) they like and input them into Yahoo Daily Contests to win $
    
    
   -----------------------------
   
      Time                             Now.or.update
      
      Yes                 Need it now for the optimizer to function
 
      Yes                 Need it now for the optimizer to function
 
      Yes                 Need it now for the optimizer to function
















