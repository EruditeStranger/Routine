# -*- coding: utf-8 -*-
"""
Created on Thu Jun 30 12:45:31 2022
This is a routine creator
@author: Metal
"""

from datetime import datetime

f = open("6th of July.txt", "a")

tasks_for_the_day = []
while True:
    task_for_the_day = input("Enter the most important things you need to get done today:\n Press 0 to quit\n")
    if task_for_the_day == "0":
        break
    else:
        tasks_for_the_day.append(task_for_the_day)

print("Here's what you said you need to get done today: ")
for i in enumerate(tasks_for_the_day):
    print(str(i))

print("Cool, let's calculate a viable schedule\n")
important_task = input("Which is the most important of these tasks for today? \n")
time_consuming_task = input("Which is the most time-consuming task for today? \n ")
easiest_task = input("Good, and what's the easiest? \n")
menial_tasks = []
while True:
    menial_task = input("Enter the other miscellaneous tasks you'd like to do today ':\n Press 0 to quit\n")
    if menial_task == "0":
        break
    else:
        menial_tasks.append(menial_task)

### Setting the current time to calculate schedule
current_time = datetime.now()
starting_hour = int(str(current_time).split(":")[0].split(" ")[1])+1
print("The current time is ", current_time , "And we're going to start working at", starting_hour , ": 00 hours")
#convert date time to string, split by ":" to get the hours (at the 0 position of the format),
#convert that to integer and add 1 to it because we'd like to give ourselves some leeway

### Finish the easiest task first ###
### Tackle the most important task second ###
### Break apart the time consuming task into chunks and repeat ###


print("Okayyyy, no maths involved yet, but here's a good outline for a schedule: \n")
print(f'{starting_hour} - {(starting_hour)+1} 00 hours: ', easiest_task, "\n")
print("30 minute break \n")
print(f'{(starting_hour)+2} - {(starting_hour)+3} 00 hours: ', important_task, "\n")
print("1 hour break\n")
print(f'{(starting_hour)+4} - {(starting_hour)+5} 00 hours: ', time_consuming_task, "Parte uno\n")
print("15 minute break")
print(f'{(starting_hour)+5} - {(starting_hour)+6} 00 hours: ', time_consuming_task, "Parte dos\n")
print("15 minute break")
print(f'{(starting_hour)+6} - {(starting_hour)+7} 00 hours: ', time_consuming_task, "Parte tres\n")
print(f"Miscellaneous tasks between ({starting_hour}+4) and ({starting_hour}+7)\n")
for i in enumerate(menial_tasks):
    print(str(i))
    
