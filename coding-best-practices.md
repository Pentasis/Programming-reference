## Returns
I'm not a "there can only be one return" purist. Multiple exit-points from a function can be preferred (e.g. using a Guard). However, I do tend to try to return at the end as much as possible. (avoiding spagetti code).

## Anonymous functions (lambda's)
Avoid them. Only use them if the function is not used anywhere else and it does not contain more than 3 lines of code max.

## One function (DRY)
Every function, method, class, module and file should do one thing or contain logical grouped code.
Better to have multiple small functions than one big function.

### Grouping caveats
Group logic based on readability over function but keep Low coupling and high cohesion in mind at all times.

## Magic numbers & Portability
Never use literals if a constant or option/setting can do.
Parameterize as much as possible and/or use settings, databases, etc.

## Boolean tests
Always implictly
e.g. if isPositive then instead of if isPositive == true then

## Comma on last item in array/list/table
Some languages don't allow this, so don't do it.
{a, b, c} NOT {a, b, c,}
