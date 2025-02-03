# Pandas.ipy
def mini(list):
  minval = list[0]
  for _ in list:
    if _ <= minval:
      minval = _
  return minval

def selection_sort(list):
  sorted_list = []
  while list:
    minval = mini(list)
    sorted_list.append(minval)
    list.remove(minval)
  return sorted_list
L1 = [14, 81, 18, 98, 56, 77]
L2 = selection_sort(L1)
print(L2)
