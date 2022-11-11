install.packages("rvest")
library(rvest)

install.packages("robotstxt")
library(robotstxt)

install.packages("xml2")
library(xml2)

install.packages("dplyr") 
library(dplyr)

install.packages("magrittr")
library(magrittr)

url<- read_html("https://www.shiksha.com/engineering/ranking/top-engineering-colleges-in-india/44-2-0-0-0")

Rank <- url %>% html_nodes(".circleText") %>% html_text()
FeeSalary <- url %>% html_nodes(".text--secondary") %>% html_text()
WeeklyRank<- url %>% html_nodes("hrzntl_flex") %>% html_text()

shikshatopunis <- data.frame(Rank, FeeSalary, WeeklyRank)
View(shikshatopunis)
