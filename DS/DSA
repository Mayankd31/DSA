#include <iostream>
using namespace std;
int a[100];
int insertion()
{
    int num;
    cout << "Enter the number you want to insert" << endl;
    cin >> num;

    int index;
    cout << "Enter the index at which you want to insert that number" << endl;
    cin >> index;

    for (int i = 4; i >= index; i--)
    {
        a[i + 1] = a[i];
    }
    a[index] = num;

    cout << "The array after insertion" << endl;
    for (int i = 0; i < 6; i++)
    {
        cout << a[i] << " ";
    }
}

int deletion()
{
    int index;
    cout << "Enter the index at which you want to delete that number" << endl;
    cin >> index;

    for (int i = index; i < 4; i++)
    {
        a[i] = a[i + 1];
    }

    cout << "The array after deletion" << endl;
    for (int i = 0; i < 4; i++)
    {
        cout << a[i] << " ";
    }
}

int sorting()
{
    for (int i = 0; i < 5; i++)
    {
        for (int j = i + 1; j < 5; j++)
        {
            if (a[i] > a[j])
            {
                int temp;
                temp = a[j];
                a[j] = a[i];
                a[i] = temp;
            }
        }
    }

    cout << "Sorted Array" << endl;
    for (int i = 0; i < 5; i++)
    {
        cout << a[i] << " ";
    }
}

int swapping()
{
    int temp, i, j;
    cout << "Enter the index you want swap with" << endl;
    cin >> i >> j;
    temp = a[i];
    a[i] = a[j];
    a[j] = temp;

    cout << "After Swapping" << endl;
    for (int i = 0; i < 5; i++)
    {
        cout << a[i] << " ";
    }
}

int traverse()
{
    cout << "After traversing" << endl;
    for (int i = 0; i < 5; i++)
    {
        cout << a[i] << " ";
    }
}

int searching()
{
    int val, flag = -1;
    cout << "Enter the number you want to search" << endl;
    cin >> val;

    for (int i = 0; i < 5; i++)
    {
        if (a[i] == val)
        {
            flag = i;
        }
    }
    if (flag != -1)
    {
        cout << "Value Found" << endl;
    }
    else
    {
        cout << "Value Not Found" << endl;
    }
}

int merging()
{
    int b[100];
    cout << "Enter the elements of 2nd array" << endl;
    for (int i = 0; i < 6; i++)
    {
        cin >> b[i];
    }

    int c[100], j = 0;
    for (int i = 0; i <= 4; i++)
    {
        c[i] = a[i];
    }

    for (int i = 5; i <= 10; i++)
    {
        c[i] = b[j];
        j++;
    }
    cout << "Array After Merging" << endl;
    for (int i = 0; i < 11; i++)
    {
        cout << c[i] << " ";
    }
}

int update()
{
    int num;
    cout << "Enter the number you want to update" << endl;
    cin >> num;

    int index;
    cout << "Enter the index at which you want to update that number" << endl;
    cin >> index;

    for (int i = 0; i < 5; i++)
    {
        a[index] = num;
    }

    cout << "After Updating the value" << endl;
    for (int i = 0; i < 5; i++)
    {
        cout << a[i] << " ";
    }
}

int append()
{
    int num;
    cout << "Enter the number you want to append" << endl;
    cin >> num;

    for (int i = 0; i < 6; i++)
    {
        a[6 + i - 1] = num;
    }

    for (int i = 0; i < 6; i++)
    {
        cout << a[i] << " ";
    }
}

int reverse()
{
    int start = 0;
    int end = 4;
    while (start <= end)
    {
        swap(a[start], a[end]);
        start++;
        end--;
    }

    cout << "The array after reversing" << endl;
    for (int i = 0; i < 5; i++)
    {
        cout << a[i] << " ";
    }
}

int sum()
{
    int sum = 0;
    for (int i = 0; i < 5; i++)
    {
        sum = sum + a[i];
    }
    cout << "After Addition" << endl;
    cout << sum << endl;
}

int product()
{
    int pro = 1;
    for (int i = 0; i < 5; i++)
    {
        pro = pro * a[i];
    }
    cout << "After Multiplication" << endl;
    cout << pro << endl;
}

int linearSearch(int a[], int key)
{

    for (int i = 0; i < 5; i++)
    {
        if (a[i] == key)
        {
            return i;
        }
    }
    return -1;
}

int binarySearch(int a[], int key1)
{
    int start = 0;
    int end = 5;
    while (start <= end)
    {
        int mid = (start + end) / 2;
        if (a[mid] == key1)
        {
            return mid;
        }
        else if (a[mid] > key1)
        {
            end = mid - 1;
        }
        else
        {
            start = mid + 1;
        }
    }
    return -1;
}

int BubbleSort()
{
    int counter = 1;
    while (counter < 5)
    {
        for (int i = 0; i < 5 - counter; i++)
        {
            if (a[i] > a[i + 1])
            {
                int temp;
                temp = a[i];
                a[i] = a[i + 1];
                a[i + 1] = temp;
            }
        }
        counter++;
    }
}

int SelectionSort()
{
    for (int i = 0; i < 4; i++)
    {
        int minIndex = i;
        for (int j = i + 1; j < 5; j++)
        {
            if (a[j] < a[minIndex])
            {
                minIndex = j;
            }
        }
        swap(a[minIndex], a[i]);
    }
}

int InsertionSort()
{
    for (int i = 1; i < 5; i++)
    {
        int temp = a[i];
        int j;
        for (j = i - 1; j >= 0; j--)
        {
            if (a[j] > temp)
            {
                // shift
                a[j + 1] = a[j];
            }
            else
            {
                break;
            }
        }
        a[j + 1] = temp;
    }
}

int main()
{
    int op;
    cout << "Enter the elements of array" << endl;
    for (int i = 0; i < 5; i++)
    {
        cin >> a[i];
    }

    cout << "Enter the operations to be performed" << endl;
    cout << "1.Insertion\n 2.Deletion\n 3.Sorting\n 4.Swapping\n 5.Traverse\n 6.Searching\n 7.Merging\n 8.Update\n 9.Append\n 10.Reverse\n  11.Sum\n 12.Product\n 13.linearSearch\n 14.binarySearch\n 15.BubbleSort\n 16.Selection Sort\n 17.InsertionSort " << endl;

    cin >> op;

    switch (op)
    {
    case 1:
        insertion();
        break;

    case 2:
        deletion();
        break;

    case 3:
        sorting();
        break;

    case 4:
        swapping();
        break;

    case 5:
        traverse();
        break;

    case 6:
        searching();
        break;

    case 7:
        merging();
        break;

    case 8:
        update();
        break;

    case 9:
        append();
        break;

    case 10:
        reverse();
        break;

    case 11:
        sum();
        break;

    case 12:
        product();
        break;

    case 13:
        int key;
        cout << "Enter the element you want to search" << endl;
        cin >> key;
        cout << linearSearch(a, key);
        break;

    case 14:
        int key1;
        cout << "Enter the element you want to search" << endl;
        cin >> key1;
        cout << binarySearch(a, key1);
        break;
    case 15:
        BubbleSort();
        cout << "Sorted Array" << endl;
        for (int i = 0; i < 5; i++)
        {
            cout << a[i] << " ";
        }
        break;
    case 16:
        SelectionSort();
        cout << "Sorted Array " << endl;
        for (int i = 0; i < 5; i++)
        {
            cout << a[i] << " ";
        }
        break;
    case 17:
        InsertionSort();
        cout << "Sorted Array " << endl;
        for (int i = 0; i < 5; i++)
        {
            cout << a[i] << " ";
        }
        break;

    default:
        cout << "Invalid choice" << endl;
    }
    return 0;
}
