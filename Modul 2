#Latihan 1
import math

def haversine(lat1, lon1, lat2, lon2):
    # Convert latitude and longitude from degrees to radians
    lat1_rad = math.radians(lat1)
    lon1_rad = math.radians(lon1)
    lat2_rad = math.radians(lat2)
    lon2_rad = math.radians(lon2)

    # Haversine formula
    dlon = lon2_rad - lon1_rad
    dlat = lat2_rad - lat1_rad
    a = math.sin(dlat / 2)**2 + math.cos(lat1_rad) * math.cos(lat2_rad) * math.sin(dlon / 2)**2
    c = 2 * math.asin(math.sqrt(a))

    # Radius of Earth in kilometers (mean radius)
    radius = 6371.0
    distance = radius * c
    return distance

# Input: Latitude and Longitude of two points
lat1 = float(input("Masukkan latitude titik 1: "))
lon1 = float(input("Masukkan longitude titik 1: "))
lat2 = float(input("Masukkan latitude titik 2: "))
lon2 = float(input("Masukkan longitude titik 2: "))

# Calculate distance
distance = haversine(lat1, lon1, lat2, lon2)

# Output: Display the distance
print(f"Jarak antara titik 1 dan titik 2 adalah: {distance:.2f} km")








#latihan 2
import math

def haversine(lat1, lon1, lat2, lon2):
    # Konversi derajat ke radian
    lat1, lon1, lat2, lon2 = map(math.radians, [lat1, lon1, lat2, lon2])
    
    # Rumus Haversine
    dlon = lon2 - lon1
    dlat = lat2 - lat1

    a = math.sin(dlat / 2)**2 + math.cos(lat1) * math.cos(lat2) * math.sin(dlon / 2)**2
    c = 2 * math.asin(math.sqrt(a))
    
    # Jarak dalam kilometer (radius Bumi sekitar 6371 km)
    r = 6371
    distance = r * c
    return distance

# Contoh penggunaan
if __name__ == "__main__":
    # Koordinat titik 1 (latitude, longitude)
    lat1 = -6.1751   # Jakarta
    lon1 = 106.8650
    # Koordinat titik 2 (latitude, longitude)
    lat2 = -7.2504   # Bandung
    lon2 = 107.7186
    
    jarak = haversine(lat1, lon1, lat2, lon2)
    print(f"Jarak antara Jakarta dan Bandung adalah: {jarak:.2f} km")
