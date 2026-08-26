
1.def login(username, password):

    if not username:
        return False

    try:
        result = request_login(username, password)

    except Exception:
        return False

    return result