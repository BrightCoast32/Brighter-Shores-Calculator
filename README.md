This calculator is designed to help players of Brighter Shores understand and plan their experience point (XP) progression, particularly in the context of the combat system after the March 6, 2025 rework.
It calculates Album XP (A) and total XP required for leveling up, based on the player's combat level (L), and can also account for XP gained from defeating monsters.

Formulas Used

The calculator relies on the following formulas for Album XP (A) and total XP, sourced from the Brighter Shores Wiki:

    For levels 0 to 799:

    A = ceil(0.3 * L^2 + ((245 + mod(2L, 5) + 5 * I) / 10) * L + 250)


L is the combat level.
mod(2L, 5) is the remainder when 2L is divided by 5.
I is an indicator variable:
    I = 1 if mod(2L, 5) < max(0, floor((L - 85) / 168) + 1)
    I = 0 otherwise
floor(x) is the greatest integer less than or equal to x.
ceil(x) is the smallest integer greater than or equal to x.


The total XP required to reach a given level is calculated using multipliers based on the level range:

Levels 0 to 5:

    XP = 2 * A

Levels 6 to 11:

    XP = 4 * A

Levels 12 to 19:

    XP = 8 * A

Levels 20 to 799:

    XP = 40 * A

For levels 800 and above:
Album XP (A) follows a simpler, linear formula:

    A = 175 * L + 250

The total XP is then:

    XP = 160 * A
