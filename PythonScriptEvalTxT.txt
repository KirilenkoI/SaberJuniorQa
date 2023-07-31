print("enter string")
def call_eval_and_input():
    math_string = str(input())
    try:
        eval(math_string)
    except:
        print("please input correct string")
        math_string = call_eval_and_input()
    return eval(str(math_string))
print(call_eval_and_input())
input("press enter to continue")
