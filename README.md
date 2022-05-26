### Hi there 👋

<!--
**Narayan1180/Narayan1180** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
I am implementing the give task in python programming language
I am using python inbuilt dictionary data structure for storing data
#"l" used for loss "w" used for win#
#
d={"GT":[20,["w","w","l","l","w"]],"LSG":[18,["w","l","l","w","w"]],"RR":[16,["w","l","w","l","l"]],"DC":[14,["w","w","l","w","l"]],"RCB":[14,["l","w","w","l","l"]],
  "KKR":[12,["l","w","w","l","w"]],"PBKS":[12,["L","W","L","W","L"]],"SRH":[12,["w","l","l","l","l"]],"CSK":[8,["l","l","w","l","w"]],"MI":[6,["l","w","l","w","w"]]}
#

printing dictionary

#

print(d)

#

retriving data using indexing and for loop

#

for i in d:
    print(i,d[i],"\n\t")

#storing filtered data in new dictionary#

d1={}
s=input("Enter String:")
n=int(input("Enter no of consecutive:"))
j=s*n
print(j)
for i in d:
    s="".join(d[i][1])
    if j in s:
        d1[i]=d[i]
        print(s)

#calculating Average of filterd list points#

total_points=0
for i in d1:
    total_points+=d1[i][0]
average=total_points/len(d1)    
print(average)  
