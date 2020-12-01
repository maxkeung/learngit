package main

import "fmt"
//二分查找,有序数组
func binaryFind(arr *[6]int,leftindex int,rightindex int,findval int ) {

	//跳出递归条件：left>right
	if leftindex>rightindex{
		fmt.Println("没找到...")
		return
	}

	middle:=(leftindex+rightindex)/2
	if findval<(*arr)[middle]{//范围在leftidnex---middleindex
		binaryFind(arr,leftindex,middle-1,findval)
	}else if findval>(*arr)[middle]{//范围在middleindex---rightindex
		binaryFind(arr,middle+1,rightindex,findval)
	}else {
		fmt.Println("找到了，下标=",middle)
	}

}

func main() {

	arr:=[6]int{-12,3,58,64,73,199}
	binaryFind(&arr,0,len(arr)-1,199)
	
}
