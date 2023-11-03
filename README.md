# BibleHomework2

The world's population is divided into sections, where each section represents an
age. For example, Section 30 has everyone who is 30 years old, Section 0 has everyone
who has just been born, and Section 72 is everyone who is about to die.

In this simulation, there can be a "fractional" amount of people, which is not very realistic, but can still be used
for easy computation. Numbers are never rounded, unless when displayed to the console.

1. Thirteen initial disciples are added into the mix before the loop starts
2. Every disciple trains 2 disciples every 3 years. Mathematically, this means that every disciple trains on average
2/3 = 0.66666 disciples per year
3. Every year, the new disciples are computed by multiplying the number of existing disciples by 2/3. Then, the new
disciples are more or less equally distributed across Sections 18 (the year people can begin training) to the oldest Section

Every year, every section's age is increased by 1. The section whose age is 72 is deleted, as they all have died. Then,
a new Section 0 is created by the number of people in Section 30. Everyone in Section 30 is assumed to be married, and
each couple has a baby, so Section 0 has (number of people in Section 30) / 2 new people.
