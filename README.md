from collections import Counter

def maxFrequencyCount(nums):
    freq = Counter(nums)
    max_freq = max(freq.values())
    return sum(count for count in freq.values() if count == max_freq)
if __name__=="__main__":
    print(maxFrequencyCount([1, 2, 2, 3, 1, 4]))  # Output: 4
    print(maxFrequencyCount([1, 2, 3, 4, 5]))     # Output: 5
