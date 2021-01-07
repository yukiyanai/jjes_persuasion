# Who Gets Close to Government Policies, and Who Steps Away?

*Japanese Journal of Electoral Studies* [選挙研究] 36(2): 139-150.

The data and materials required to verify the computational reproducibility of the results, procedures, and analyses in the article.

## Authors

- [Sohei Shigemura](https://soheishigemura.com/), Kobe University
- [Jaehyun Song](https://www.jaysong.net/), Doshisha University
- [Yuki Yanai](https://yukiyanai.github.io/), Kochi University of Technology


## Abstract

We investigate how political elites shape public opinion. The literature of opinion leadership has paid considerable attention to how politicians influence their constituents' policy preferences. Some show that elites can shift their supporters' positions by merely announcing the elites' positions.  Others assert that politicians' position-taking does not change voters' positions, but that they can persuade voters to believe that the proposed policies are beneficial. By analyzing an original data set from a survey experiment in Japan, we reveal when the government succeeds in shaping public opinion and when it fails. Combining randomized framing and a conjoint experiment, we find that persuasion works when the prime minister provides ideologically well-aligned justification. Moreover, the persuasion effect is attenuated when the persuader takes an ideologically contradictory position. Our study highlights the influence of Prime Minister Shinzo Abe and contributes to a better understanding of political communication between elites and voters.

## Data

The data to reproduce the results presented in the article are in the following CSV file. The data set is in the form to be anlayzed as conjoint data, which means that each row does *not* repsent a respondent. Rather, each row is a respondent's reaction to a specific profile in a specific task in the conojoint experiment. In other words, each respondent appears in multiple rows.

- [jjes2020_ShigemuraSongYanai.csv](jjes2020_ShigemuraSongYanai.csv)

### Variables

The data set contains the following variables.

- Group: Identifies the experimental condition shown in Table 2 of the article (p.144).
- ID: Identifies the respondent. Each repondent has a unique ID.
- task: Task number of the conjoint experiment. An integer between 1 and 5.
- profile: Profile number of each task in the conjoint experiment. 1 or 2.
- selected: Indicates whether a profile is selected (1) or not (0).
- temp_Abe: Feeling thermometer rating for Prime Minister Shinzo Abe. Ranges from 0 to 100 (integer).

The following six variables are the attributes used in our conjoint experiment. Please see Table 1 of the article (p.144) for detail.

- emperor: Female emperor.
- immigrants: Immigration.
- childcare: Childcare.
- tax: Consumption tax.
- party: Party affiliation.
- age_candidate: Age
- gender_candidate: Gender.
- status: Status.


## R Codes

R codes to reproduce the results presented in the article are available in the following R Markdown and HTML files.

- [replication_jjes2020_SSY.Rmd](replication_jjes2020_SSY.Rmd)
- [replication_jjes2020_SSY.html](replication_jjes2020_SSY.html)