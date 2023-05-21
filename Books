import qrcode

n=int(input('No of Records to be Inserted : '))

for i in range(n):

    b90 = input('Owner : ') # ID

    b89 = input('Date Purchased : ')

    b91 = input('Book Name  : ') # Name

    b92 = input('Author : ') # Author

    b93 = input('Publisher : ') # Post

    b94 = input('Book Code : ') # Book Code

    b95 = input('Date Finished : ') # Date Finished
 
    import mysql.connector as sql
    con=sql.connect(host='localhost',user='root',password='dayem',database='book')
    cur=con.cursor()

    query='INSERT INTO DETAILS VALUES (%s,%s,%s,%s,%s,%s,%s)'
    values=(b90,b89,b91,b92,b93,b94,b95)

    cur.execute(query,values)
    con.commit()

    data=(b90,b89,b91,b92,b95)

    img=qrcode.make(data)

    qr55=b91+' '+b92+'.jpeg'

    img.save(qr55)

    print(qr55)
