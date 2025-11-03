###############################################################
# LABORATORIUM 4
# Autor: Michal Wojtowicz
# Grupa: 2.4
###############################################################
# --- URUCHOMIENIE PODA ---
kubectl apply -f loop-pod.yaml

# Sprawdź status Poda
kubectl get pods

# Wyświetl logi z kontenera
kubectl logs loop

# Pod po zakończeniu pętli przechodzi w stan Completed.
# --- USUNIĘCIE POPRZEDNIEGO PODA ---
kubectl delete pod loop

# --- URUCHOMIENIE ZMODYFIKOWANEGO PODA ---
kubectl apply -f loop-pod-running.yaml

# Sprawdź status Poda (Running)
kubectl get pod loop

# --- SPRAWDZENIE LOGÓW ---
kubectl logs loop
