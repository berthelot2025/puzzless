


<script>
export default {
  name: "Records-component",
  data() {
    return {
      records: [],
    };
  },
  created() {
    this.getRecords();
  },
  methods: {
    getRecords() {
      const records = JSON.parse(localStorage.getItem("records")) || [];
      this.records = records;
    },
  },
};
</script>
