#include <iostream>
using namespace std; 
int main() { 
	int ms, ps, nop, mp[10], n; 
	cout << "Enter total memory size: "; 
	cin >> ms;
cout << "Enter partition size: ";
cin >> ps; 
n = ms / ps;
cout << "Total partitions: " << n << endl;
cout << "Enter number of processes: "; 
cin >> nop; 
for (int i = 0; i < nop; i++) { 
	cout << "Enter memory required for process " << i+1 << ": "; 
	cin >> mp[i]; 
} 
for (int i = 0; i < nop && i < n; i++) { 	if (mp[i] <= ps)
cout << "Process " << i+1 << " allocated in partition " << i+1 
<< " with internal fragmentation: " << ps - mp[i] << endl;
else
		cout << "Process " << i+1 << " not allocated (too large)." << endl; 	} 
	return 0; 
}
