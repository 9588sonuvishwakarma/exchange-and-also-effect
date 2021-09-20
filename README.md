# exchange-and-also-effect
you can change the functio
a = 1
b = 9
a,b =b,a

temp = a
a = b
b = temp

temp = a
a = b
b = temp

print(a)


def div(a,b):
    print(a-b)

def smart_div(si):
    def inner(a,b):
        if a>b:
            a,b = b,a
        return si (a,b)
    return inner
div = smart_div(div)


div(8,6)


