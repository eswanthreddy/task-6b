# task-6b
def count_error_lines(filename):
    """Count the number of lines that contain the word 'ERROR'."""
    error_count = 0
    with open(filename, "r") as file:
        for line in file:
            if "ERROR" in line.upper():  # Case-insensitive check for 'ERROR'
                error_count += 1
    return error_count

# Call the function and print the result
error_lines = count_error_lines("log.txt")
print(f"Number of lines with 'ERROR': {error_lines}")


