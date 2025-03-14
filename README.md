# Iterative-Search

Search(Iterative)

Search for a key in a Linked List. Return the position where it is found. If not found, return -1.

public int itrSearch(int key) {
        Node temp = head;
        int i = 0;

        while (temp != null) {
            if (temp.data == key) { // key found
                return i;
            }
            temp = temp.next;
            i++;
        }
        //key not found
        return -1;
    }