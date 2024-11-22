# Max-Free-Days-at-Camp

Naina is attending a camp that lasts for N days, and she has a list of M destinations she wants to explore. Each destination requires a certain number of days, Ai, to fully experience. Since she can only visit one destination per day and can’t take a day off while exploring, Naina wonders how many free days she’ll have left to relax if she completes all her visits. If it’s not possible for her to visit all destinations within the camp duration, return -1.

def max_free_days(n, m, days):

    total_required = sum(days)
    if total_required > n:
        return -1
    return n - total_required

# Input reading
n, m = map(int, input().split())
days = list(map(int, input().split()))

# Output result
print(max_free_days(n, m, days))
