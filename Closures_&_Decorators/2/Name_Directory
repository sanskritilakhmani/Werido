
## Decorators 2 - Name Directory
import operator

# Option 1
def person_lister(f):
    def inner(people):
        # complete the function
        return map(f, sorted(people, key=lambda x: int(x[2]))) 
    return inner

# # Option 2
# def person_lister(f):
#     def inner(people):
#         g=[]
#         people= sorted (people, key=lambda x : int(x[2]))
#         for i in people:
#             g.append(f(i))
#         people=g
#         return people
#     return inner

@person_lister
def name_format(person):
    return ("Mr. " if person[3] == "M" else "Ms. ") + person[0] + " " + person[1]

if __name__ == '__main__':
    people = [input().split() for i in range(int(input()))]
    print(*name_format(people), sep='\n')


## end ##
