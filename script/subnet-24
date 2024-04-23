from pythonping import ping

# Définir la plage d'adresses IP
ip_base = "10.192.1."
ip_start = 1
ip_end = 253

# Pinger chaque adresse dans la plage
for i in range(ip_start, ip_end + 1):
    ip_address = ip_base + str(i)
    response = ping(ip_address, count=1, timeout=1)  # Envoie un seul ping avec un timeout de 1 seconde
    if response.success():
        print(f"{ip_address} is up")
    else:
        print(f"{ip_address} is down")
