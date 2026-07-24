# TP-vlan---mode-trunkts continuité du TP vlan.

objectif: le mode trunk est une configuration appliquée à un port de switch qui lui permet de faire passer le trafic de plusieurs vlans différents à travers un seul et unique câble physique. ( Backone)


puisque j'avais déja configuré les ip dans la prémiere topologie vlan ici; j'ai fait que configuré le mode trunk sur le commutateur 1 et le commutateur 2


sur le commutateur 0:
enable 
configure terminal
interface gigabitethernet 0/1 
switchport mode trunk
end
write

sur le commutateur 1:
enable
configure terminal
interface gigabitethernet 0/1
switchport mode trunk
end
write


pour ma vérification: 
show interfaces trunk
