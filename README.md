# sign_lang
sign language with ASL system 
REQURIMENT
install tesnsorflow
install numpy


First step (train the data set)
in the terminal we write 
python3 train.py \
  --bottleneck_dir=logs/bottlenecks \
  --how_many_training_steps=2000 \
  --summaries_dir=logs/training_summaries/basic \
  --output_graph=logs/trained_graph.pb \
  --output_labels=logs/trained_labels.txt \
  --image_dir=./dataset


** it will take from 15-mins to couple of hours depend on your data set 

Second step (test the NN)

python3 classify.py test_image_path.jpg

it will give you output like (it was tested for M )
m (score = 0.18646)
a (score = 0.14670)
n (score = 0.12052)
o (score = 0.07318)
b (score = 0.05841)
w (score = 0.05272)
s (score = 0.05244)
e (score = 0.03675)
u (score = 0.03002)
r (score = 0.02912)
k (score = 0.02654)
q (score = 0.02292)
p (score = 0.02099)
y (score = 0.02038)
nothing (score = 0.01745)
del (score = 0.01702)
c (score = 0.01464)
v (score = 0.01272)
x (score = 0.01125)
d (score = 0.00654)
space (score = 0.00600)
f (score = 0.00597)
l (score = 0.00573)
i (score = 0.00528)
h (score = 0.00500)
g (score = 0.00490)
t (score = 0.00475)
z (score = 0.00291)
j (score = 0.00271)

you will find the data and trained lables 
*** the network was tested in other images but did't give such an accuert result so 
I guess it need more data and training 
