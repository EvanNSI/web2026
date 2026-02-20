#1 
mkdir tpLinux

#2 
tree 

#3
touch fic1.txt
touch fic2.txt
touch fichier.md
touch image.jpg
touch exos.md
touch exoos.txt

#4
mkdir dosA
mkdir dosD
cd ./dosA
mkdir dosB
mkdir dosC

#5
mv ./fi* ./dosA/dosB

#6
cd ../
cp ./fic1.txt ./dosA/dosB
cp ./fic2.txt ./dosA/dosC
cp ./fichier.md ./dosD

#7
cd ../
cd ./fic1.txt
echo "bonjour tout le monde"


#8
find ./ -name "

#9
mv ./exoos.txt ./exos.txt

#10
cd ../
touch supprimer.sh 
cd ./ supprimer.sh
rm -r ./tpLinux 
chmod 100 ./supprimer.sh