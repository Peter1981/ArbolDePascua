import matplotlib.pyplot as plt
import numpy as np

z = np.arange(0, 1, 0.03)
theta = np.arange(0, 2*np.pi + np.pi/50, np.pi/50)

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')
radius=0.7

for j in z:
	x = radius*j * np.array([np.cos(q) for q in theta])
	y = radius*j * np.array([np.sin(q) for q in theta])
	ax.plot(x, y, -j, 'g-')
	
x1 = radius*z * np.sin(20 * z)
y1 = radius*z * np.cos(20 * z)
for j in range(1,len(x1)+1):
	if j%2==0:
		ax.plot(x1[j-1],y1[j-1],-z[j-1],'ro')
	else:
		ax.plot(x1[j-1],y1[j-1],-z[j-1],'yo')
		
ax.set_title('Feliz Navidad',fontsize=26)
plt.show()
