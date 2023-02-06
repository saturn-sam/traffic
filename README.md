I have tested with multiple set of parameters. I have mentioned with the steps bellow.
step 1:
	- Convolutional layer: 1
	- Max-pooling layer: 1
		- pool_size: 2x2
	- hidden layer: 1
		- nodes: 256
	- Dropout layer: 1
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 15s 14ms/step - loss: 4.6228 - accuracy: 0.0524
Epoch 2/10
500/500 [==============================] - 7s 14ms/step - loss: 3.5894 - accuracy: 0.0561
Epoch 3/10
500/500 [==============================] - 7s 14ms/step - loss: 3.5413 - accuracy: 0.0576
Epoch 4/10
500/500 [==============================] - 7s 14ms/step - loss: 3.5185 - accuracy: 0.0576
Epoch 5/10
500/500 [==============================] - 7s 14ms/step - loss: 3.5081 - accuracy: 0.0576
Epoch 6/10
500/500 [==============================] - 7s 14ms/step - loss: 3.5032 - accuracy: 0.0576
Epoch 7/10
500/500 [==============================] - 7s 13ms/step - loss: 3.5008 - accuracy: 0.0576
Epoch 8/10
500/500 [==============================] - 7s 14ms/step - loss: 3.4997 - accuracy: 0.0576
Epoch 9/10
500/500 [==============================] - 7s 13ms/step - loss: 3.4991 - accuracy: 0.0576
Epoch 10/10
500/500 [==============================] - 7s 13ms/step - loss: 3.4988 - accuracy: 0.0576
333/333 - 37s - loss: 3.4980 - accuracy: 0.0544 - 37s/epoch - 112ms/step


step 2:
	- Convolutional layer: 1
	- Max-pooling layer: 1
		- pool_size: 2x2
	- hidden layer: 2 <-----------------
		- nodes: 256
	- Dropout layer: 1
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 13s 24ms/step - loss: 4.0410 - accuracy: 0.3834
Epoch 2/10
500/500 [==============================] - 12s 24ms/step - loss: 0.9218 - accuracy: 0.7462
Epoch 3/10
500/500 [==============================] - 12s 23ms/step - loss: 0.5669 - accuracy: 0.8455
Epoch 4/10
500/500 [==============================] - 11s 23ms/step - loss: 0.4001 - accuracy: 0.8920
Epoch 5/10
500/500 [==============================] - 12s 23ms/step - loss: 0.3379 - accuracy: 0.9116
Epoch 6/10
500/500 [==============================] - 12s 23ms/step - loss: 0.2838 - accuracy: 0.9251
Epoch 7/10
500/500 [==============================] - 12s 23ms/step - loss: 0.2848 - accuracy: 0.9267
Epoch 8/10
500/500 [==============================] - 12s 23ms/step - loss: 0.2716 - accuracy: 0.9349
Epoch 9/10
500/500 [==============================] - 11s 23ms/step - loss: 0.1909 - accuracy: 0.9524
Epoch 10/10
500/500 [==============================] - 12s 23ms/step - loss: 0.2835 - accuracy: 0.9331
333/333 - 1s - loss: 0.3511 - accuracy: 0.9208 - 1s/epoch - 4ms/step



step 3:
	- Convolutional layer: 2 <----------
	- Max-pooling layer: 2 <-------------
		- pool_size: 2x2
	- hidden layer: 2
		- nodes: 256
	- Dropout layer: 1
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 8s 13ms/step - loss: 2.4698 - accuracy: 0.4429
Epoch 2/10
500/500 [==============================] - 7s 13ms/step - loss: 0.7472 - accuracy: 0.7852
Epoch 3/10
500/500 [==============================] - 7s 13ms/step - loss: 0.3980 - accuracy: 0.8867
Epoch 4/10
500/500 [==============================] - 7s 13ms/step - loss: 0.2621 - accuracy: 0.9274
Epoch 5/10
500/500 [==============================] - 7s 13ms/step - loss: 0.2262 - accuracy: 0.9383
Epoch 6/10
500/500 [==============================] - 7s 13ms/step - loss: 0.1885 - accuracy: 0.9489
Epoch 7/10
500/500 [==============================] - 7s 14ms/step - loss: 0.1452 - accuracy: 0.9608
Epoch 8/10
500/500 [==============================] - 7s 13ms/step - loss: 0.1215 - accuracy: 0.9687
Epoch 9/10
500/500 [==============================] - 7s 13ms/step - loss: 0.1516 - accuracy: 0.9595
Epoch 10/10
500/500 [==============================] - 7s 13ms/step - loss: 0.1250 - accuracy: 0.9688
333/333 - 1s - loss: 0.1836 - accuracy: 0.9598 - 1s/epoch - 4ms/step


step 3:
	- Convolutional layer: 2
		- conv layer kernel size: 3x3
	- Max-pooling layer: 2
		- pool_size: 3x3 <-----------------
	- hidden layer: 2
		- nodes: 256
	- Dropout layer: 1
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 5s 8ms/step - loss: 3.2663 - accuracy: 0.2472
Epoch 2/10
500/500 [==============================] - 4s 8ms/step - loss: 1.6510 - accuracy: 0.5020
Epoch 3/10
500/500 [==============================] - 4s 8ms/step - loss: 1.2677 - accuracy: 0.6002
Epoch 4/10
500/500 [==============================] - 4s 8ms/step - loss: 1.0191 - accuracy: 0.6767
Epoch 5/10
500/500 [==============================] - 4s 8ms/step - loss: 0.8470 - accuracy: 0.7325
Epoch 6/10
500/500 [==============================] - 4s 8ms/step - loss: 0.7196 - accuracy: 0.7741
Epoch 7/10
500/500 [==============================] - 4s 8ms/step - loss: 0.5867 - accuracy: 0.8118
Epoch 8/10
500/500 [==============================] - 4s 8ms/step - loss: 0.5169 - accuracy: 0.8408
Epoch 9/10
500/500 [==============================] - 4s 8ms/step - loss: 0.4637 - accuracy: 0.8580
Epoch 10/10
500/500 [==============================] - 4s 8ms/step - loss: 0.3969 - accuracy: 0.8773
333/333 - 1s - loss: 0.4409 - accuracy: 0.8666 - 1s/epoch - 3ms/step


step 4:
	- Convolutional layer: 2
		- conv layer kernel size: 3x3
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3<---------------
		- nodes: 256
	- Dropout layer: 1
		- Dropout: .5

Epoch 1/10
500/500 [==============================] - 8s 14ms/step - loss: 2.4490 - accuracy: 0.4515
Epoch 2/10
500/500 [==============================] - 7s 14ms/step - loss: 0.6310 - accuracy: 0.8162
Epoch 3/10
500/500 [==============================] - 7s 14ms/step - loss: 0.3583 - accuracy: 0.9011
Epoch 4/10
500/500 [==============================] - 7s 14ms/step - loss: 0.2516 - accuracy: 0.9278
Epoch 5/10
500/500 [==============================] - 7s 14ms/step - loss: 0.2200 - accuracy: 0.9428
Epoch 6/10
500/500 [==============================] - 7s 14ms/step - loss: 0.1601 - accuracy: 0.9565
Epoch 7/10
500/500 [==============================] - 7s 14ms/step - loss: 0.1696 - accuracy: 0.9574
Epoch 8/10
500/500 [==============================] - 7s 14ms/step - loss: 0.1307 - accuracy: 0.9658
Epoch 9/10
500/500 [==============================] - 7s 14ms/step - loss: 0.1278 - accuracy: 0.9668
Epoch 10/10
500/500 [==============================] - 7s 14ms/step - loss: 0.1645 - accuracy: 0.9596
333/333 - 1s - loss: 0.1836 - accuracy: 0.9628 - 1s/epoch - 4ms/step


step 5:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 256
	- Dropout layer: 1
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 7s 12ms/step - loss: 2.4169 - accuracy: 0.4057
Epoch 2/10
500/500 [==============================] - 6s 12ms/step - loss: 0.8512 - accuracy: 0.7454
Epoch 3/10
500/500 [==============================] - 6s 12ms/step - loss: 0.4628 - accuracy: 0.8583
Epoch 4/10
500/500 [==============================] - 6s 12ms/step - loss: 0.3182 - accuracy: 0.9082
Epoch 5/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2205 - accuracy: 0.9368
Epoch 6/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2085 - accuracy: 0.9408
Epoch 7/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1726 - accuracy: 0.9520
Epoch 8/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1517 - accuracy: 0.9590
Epoch 9/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1422 - accuracy: 0.9623
Epoch 10/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1061 - accuracy: 0.9722
333/333 - 1s - loss: 0.2018 - accuracy: 0.9498 - 1s/epoch - 4ms/step


step 6:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 256
	- Dropout layer: 3 <------------------
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 7s 12ms/step - loss: 4.3645 - accuracy: 0.1064
Epoch 2/10
500/500 [==============================] - 6s 12ms/step - loss: 2.6623 - accuracy: 0.2825
Epoch 3/10
500/500 [==============================] - 6s 12ms/step - loss: 2.2235 - accuracy: 0.3525
Epoch 4/10
500/500 [==============================] - 6s 12ms/step - loss: 1.9601 - accuracy: 0.3966
Epoch 5/10
500/500 [==============================] - 6s 12ms/step - loss: 1.7813 - accuracy: 0.4240
Epoch 6/10
500/500 [==============================] - 6s 12ms/step - loss: 1.6740 - accuracy: 0.4533
Epoch 7/10
500/500 [==============================] - 6s 12ms/step - loss: 1.6081 - accuracy: 0.4702
Epoch 8/10
500/500 [==============================] - 6s 12ms/step - loss: 1.4966 - accuracy: 0.5026
Epoch 9/10
500/500 [==============================] - 6s 12ms/step - loss: 1.3843 - accuracy: 0.5350
Epoch 10/10
500/500 [==============================] - 6s 12ms/step - loss: 1.3108 - accuracy: 0.5609
333/333 - 1s - loss: 0.9904 - accuracy: 0.6835 - 1s/epoch - 4ms/step

step 7:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 4
		- nodes: 256
	- Dropout layer: 1 <--------------------
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 7s 12ms/step - loss: 2.4737 - accuracy: 0.3850
Epoch 2/10
500/500 [==============================] - 6s 12ms/step - loss: 0.8080 - accuracy: 0.7594
Epoch 3/10
500/500 [==============================] - 6s 12ms/step - loss: 0.4449 - accuracy: 0.8702
Epoch 4/10
500/500 [==============================] - 6s 12ms/step - loss: 0.3324 - accuracy: 0.9083
Epoch 5/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2530 - accuracy: 0.9297
Epoch 6/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2046 - accuracy: 0.9454
Epoch 7/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1793 - accuracy: 0.9528
Epoch 8/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1314 - accuracy: 0.9655
Epoch 9/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1609 - accuracy: 0.9583
Epoch 10/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1341 - accuracy: 0.9662
333/333 - 1s - loss: 0.2180 - accuracy: 0.9527 - 1s/epoch - 4ms/step

step 8:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3<----------
		- nodes: 512<---------------
	- Dropout layer: 1
		- Dropout: .5
		
Epoch 1/10
500/500 [==============================] - 11s 21ms/step - loss: 1.9927 - accuracy: 0.5170
Epoch 2/10
500/500 [==============================] - 10s 21ms/step - loss: 0.5987 - accuracy: 0.8255
Epoch 3/10
500/500 [==============================] - 10s 21ms/step - loss: 0.3637 - accuracy: 0.8954
Epoch 4/10
500/500 [==============================] - 10s 20ms/step - loss: 0.2677 - accuracy: 0.9285
Epoch 5/10
500/500 [==============================] - 10s 20ms/step - loss: 0.2033 - accuracy: 0.9421
Epoch 6/10
500/500 [==============================] - 10s 20ms/step - loss: 0.1969 - accuracy: 0.9489
Epoch 7/10
500/500 [==============================] - 10s 21ms/step - loss: 0.1582 - accuracy: 0.9588
Epoch 8/10
500/500 [==============================] - 10s 21ms/step - loss: 0.1849 - accuracy: 0.9549
Epoch 9/10
500/500 [==============================] - 10s 21ms/step - loss: 0.1555 - accuracy: 0.9621
Epoch 10/10
500/500 [==============================] - 10s 20ms/step - loss: 0.1541 - accuracy: 0.9634
333/333 - 2s - loss: 0.3899 - accuracy: 0.9273 - 2s/epoch - 5ms/step

step 9:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 256<---------------
	- Dropout layer: 1
		- Dropout: .3<--------------

Epoch 1/10
500/500 [==============================] - 7s 12ms/step - loss: 2.0516 - accuracy: 0.5195
Epoch 2/10
500/500 [==============================] - 6s 12ms/step - loss: 0.5958 - accuracy: 0.8243
Epoch 3/10
500/500 [==============================] - 6s 12ms/step - loss: 0.3769 - accuracy: 0.8910
Epoch 4/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2773 - accuracy: 0.9244
Epoch 5/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2149 - accuracy: 0.9389
Epoch 6/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1783 - accuracy: 0.9491
Epoch 7/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1505 - accuracy: 0.9583
Epoch 8/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1311 - accuracy: 0.9634
Epoch 9/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1539 - accuracy: 0.9616
Epoch 10/10
500/500 [==============================] - 6s 12ms/step - loss: 0.1326 - accuracy: 0.9655
333/333 - 1s - loss: 0.2080 - accuracy: 0.9521 - 1s/epoch - 4ms/step

step 10:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 128<---------------
	- Dropout layer: 1
		- Dropout: .5<--------------
		
Epoch 1/10
500/500 [==============================] - 5s 9ms/step - loss: 2.8240 - accuracy: 0.3132
Epoch 2/10
500/500 [==============================] - 5s 9ms/step - loss: 1.1606 - accuracy: 0.6444
Epoch 3/10
500/500 [==============================] - 5s 9ms/step - loss: 0.7248 - accuracy: 0.7777
Epoch 4/10
500/500 [==============================] - 5s 10ms/step - loss: 0.4965 - accuracy: 0.8490
Epoch 5/10
500/500 [==============================] - 5s 9ms/step - loss: 0.3547 - accuracy: 0.8950
Epoch 6/10
500/500 [==============================] - 5s 10ms/step - loss: 0.2848 - accuracy: 0.9171
Epoch 7/10
500/500 [==============================] - 5s 10ms/step - loss: 0.2660 - accuracy: 0.9222
Epoch 8/10
500/500 [==============================] - 5s 10ms/step - loss: 0.1963 - accuracy: 0.9449
Epoch 9/10
500/500 [==============================] - 5s 9ms/step - loss: 0.1643 - accuracy: 0.9551
Epoch 10/10
500/500 [==============================] - 5s 9ms/step - loss: 0.1690 - accuracy: 0.9535
333/333 - 1s - loss: 0.1651 - accuracy: 0.9590 - 1s/epoch - 4ms/step

step 11:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 256,128,128<---------------
		
	- Dropout layer: 1
		- Dropout: .5<--------------
		
Epoch 1/10
500/500 [==============================] - 7s 12ms/step - loss: 2.6523 - accuracy: 0.3425
Epoch 2/10
500/500 [==============================] - 6s 11ms/step - loss: 1.0579 - accuracy: 0.6760
Epoch 3/10
500/500 [==============================] - 6s 11ms/step - loss: 0.6243 - accuracy: 0.8081
Epoch 4/10
500/500 [==============================] - 6s 11ms/step - loss: 0.4133 - accuracy: 0.8754
Epoch 5/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2944 - accuracy: 0.9139
Epoch 6/10
500/500 [==============================] - 6s 11ms/step - loss: 0.2537 - accuracy: 0.9281
Epoch 7/10
500/500 [==============================] - 6s 12ms/step - loss: 0.2106 - accuracy: 0.9403
Epoch 8/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1656 - accuracy: 0.9527
Epoch 9/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1762 - accuracy: 0.9525
Epoch 10/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1425 - accuracy: 0.9595
333/333 - 1s - loss: 0.1837 - accuracy: 0.9549 - 1s/epoch - 4ms/step




step 12:
	- Convolutional layer: 2
		- conv layer kernel size: 2x2
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 256,128,128<---------------
		
	- Dropout layer: 1
		- Dropout: .5<--------------


Epoch 1/10
500/500 [==============================] - 7s 12ms/step - loss: 2.9998 - accuracy: 0.2909
Epoch 2/10
500/500 [==============================] - 6s 11ms/step - loss: 1.1999 - accuracy: 0.6343
Epoch 3/10
500/500 [==============================] - 6s 12ms/step - loss: 0.6424 - accuracy: 0.8078
Epoch 4/10
500/500 [==============================] - 6s 11ms/step - loss: 0.4253 - accuracy: 0.8704
Epoch 5/10
500/500 [==============================] - 6s 11ms/step - loss: 0.3158 - accuracy: 0.9097
Epoch 6/10
500/500 [==============================] - 6s 11ms/step - loss: 0.2366 - accuracy: 0.9332
Epoch 7/10
500/500 [==============================] - 6s 11ms/step - loss: 0.2015 - accuracy: 0.9414
Epoch 8/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1892 - accuracy: 0.9470
Epoch 9/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1858 - accuracy: 0.9499
Epoch 10/10
500/500 [==============================] - 6s 11ms/step - loss: 0.1722 - accuracy: 0.9563
333/333 - 1s - loss: 0.1285 - accuracy: 0.9669 - 1s/epoch - 4ms/step


step 12:
	- Convolutional layer: 2
		- conv layer kernel size: 3x3
		- filter: 64,128
	- Max-pooling layer: 2
		- pool_size: 2x2
	- hidden layer: 3
		- nodes: 256,128,128<---------------
		
	- Dropout layer: 1
		- Dropout: .5<--------------

Epoch 1/10
500/500 [==============================] - 18s 33ms/step - loss: 2.1833 - accuracy: 0.4546
Epoch 2/10
500/500 [==============================] - 17s 34ms/step - loss: 0.6046 - accuracy: 0.8317
Epoch 3/10
500/500 [==============================] - 17s 34ms/step - loss: 0.3095 - accuracy: 0.9147
Epoch 4/10
500/500 [==============================] - 17s 34ms/step - loss: 0.2228 - accuracy: 0.9409
Epoch 5/10
500/500 [==============================] - 17s 34ms/step - loss: 0.1424 - accuracy: 0.9636
Epoch 6/10
500/500 [==============================] - 17s 34ms/step - loss: 0.1676 - accuracy: 0.9585
Epoch 7/10
500/500 [==============================] - 17s 34ms/step - loss: 0.1345 - accuracy: 0.9688
Epoch 8/10
500/500 [==============================] - 17s 34ms/step - loss: 0.1695 - accuracy: 0.9621
Epoch 9/10
500/500 [==============================] - 17s 34ms/step - loss: 0.1557 - accuracy: 0.9676
Epoch 10/10
500/500 [==============================] - 17s 34ms/step - loss: 0.0997 - accuracy: 0.9785
333/333 - 2s - loss: 0.1148 - accuracy: 0.9771 - 2s/epoch - 7ms/step