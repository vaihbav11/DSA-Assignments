class Solution:
    def detectCycle(self, head):
        slow = head
        fast = head

        # Phase 1: detect cycle 
        while fast and fast.next:
            slow = slow.next
            fast = fast.next.next

            if slow == fast:
                # Phase 2: find cycle start
                pointer = head
                while pointer != slow:
                    pointer = pointer.next
                    slow = slow.next
                return pointer  # this is the cycle start node

        return None  # no cycle
