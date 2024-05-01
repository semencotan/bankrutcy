# bankrutcy
def check_bankruptcy(total_assets, total_liabilities, threshold):
    net_worth = total_assets - total_liabilities
    if net_worth < threshold:
        return True  # Bankruptcy
    else:
        return False  # Not bankrupt

# Example usage
if __name__ == "__main__":
    total_assets = 50000  # Total assets
    total_liabilities = 75000  # Total liabilities
    threshold = 0  # Threshold for bankruptcy (negative net worth)

    is_bankrupt = check_bankruptcy(total_assets, total_liabilities, threshold)
    if is_bankrupt:
        print("You are bankrupt!")
    else:
        print("You are not bankrupt.")
