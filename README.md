def get_adult_users(users):
    # users is a list of dictionaries: [{'name': 'Aayush', 'age': 21}, ...]
    adults = [user['name'] for user in users if user['age'] > 18]
    return adults

# Example usage:
users = [
    {'name': 'Aayush', 'age': 21},
    {'name': 'Riya', 'age': 17},
    {'name': 'Arjun', 'age': 19}
]
print(get_adult_users(users))  # Output: ['Aayush', 'Arjun']
