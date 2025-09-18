# my-first-project
def stress_level(sleep_hours, workload, caffeine):
    score = 0
    
    if sleep_hours < 6:
        score += 2
    elif sleep_hours < 8:
        score += 1

    if workload == "heavy":
        score += 2
    elif workload == "medium":
        score += 1

    if caffeine == "high":
        score += 1

    if score <= 2:
        return "Low Stress"
    elif score <= 4:
        return "Medium Stress"
    else:
        return "High Stress"

# Example usage
print(stress_level(5, "heavy", "high"))   # High Stress
print(stress_level(7, "medium", "low"))   # Medium Stress
print(stress_level(8, "light", "low"))    # Low Stress

