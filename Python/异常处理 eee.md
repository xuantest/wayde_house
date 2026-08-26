def login(username, password):

    if not username:
        return False

    try:
        result = request_login(username, password)

    except Exception:
        return False

    return result
'''
1.username 为空时返回False
2.except 扑获异常报错则执行False
'''