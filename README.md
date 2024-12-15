# pyuygulama2
import math
# Öklid mesafesini hesaplayan fonksiyon
def euclideanDistance(point1, point2):
    return math.sqrt((point2[0] - point1[0])**2 + (point2[1] - point1[1])**2)

# 2D uzaydaki noktaları temsil eden liste
points = [(1, 2), (4, 6), (5, 7), (8, 9), (2, 3)]

# Tüm mesafeleri saklıyoruz
distances = []

# Tüm nokta çiftleri arasındaki mesafeleri hesaplama
for x in range(len(points)):
    for y in range(i + 1, len(points)):  # Aynı noktayı iki kez karşılaştırmamak için i+1'den başlıyoruz
        distance = euclideanDistance(points[x], points[y])
        distances.append(distance)
        print(f"Mesafe {points[x]} ile {points[y]} arasında: {distance:.2f}")

# Minimum mesafe
minimum_distance = min(distances)

# Minimum mesafeyi yazdırma
print(f"\nEn kısa mesafe: {minimum_distance:.2f}")
