#include <iostream>
#include <queue>
#include <vector>
using namespace std; 
int main() { 
	int n, f, page, faults = 0; 
	cout << "Enter number of frames: "; 
	cin >> f; 
	cout << "Enter number of pages: "; 
	cin >> n; 
	vector<int> pages(n); 
	cout << "Enter reference string: "; 
	for (int i = 0; i < n; i++) cin >> pages[i]; 
	queue<int> q; 
	vector<int> frame; 
	for (int i = 0; i < n; i++) { 
		page = pages[i]; 
		bool found = false; 
		for (int x : frame) if (x == page) found = true; 
		if (!found) { 
			if (frame.size() < f) frame.push_back(page); 
			else {
int victim = q.front(); q.pop();
for (int j = 0; j < frame.size(); j++)
if (frame[j] == victim) frame[j] = page;
			} 
		q.push(page); 
		faults++; 
		} 
		cout << "Frames: "; 
		for (int x : frame) cout << x << " "; 
		cout << endl; 
	} 
	cout << "Total Page Faults: " << faults << endl; 
	return 0; 
}
